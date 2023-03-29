# Sending email by SMTP Protocol

To send an e-mail, up the server on port 8080 e make a `POST` request on the following URL, with the following parameters:

`localhost:8080/sending-email`

```json
{
	"ownerRef": "John Doe",
	"emailFrom": "johndoe@example.com",
	"emailTo": "example@example.com",
	"subject": "Hello, Java!",
	"text": "Hello, World"
}
```

It's necessary to configure the following variables into `application.properties` file.
```
spring.mail.username=example@gmail.com
spring.mail.password=1234567891011123
```

Also, it's necessary to get the google code with 16 characters to configure the SMTP protocol. To generate the code, following the steps on this tutorial: `https://support.google.com/accounts/answer/185833`