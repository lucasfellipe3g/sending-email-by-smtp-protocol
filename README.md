# Sending email

Para enviar um e-mail, suba o servidor na porta 8080 e faça um `POST` na seguinte URL passando os seguintes parâmetros:

`localhost:8080/sending-email`

```json
{
	"ownerRef": "Lucas Fellipe",
	"emailFrom": "lucas.fellipe.c@gmail.com",
	"emailTo": "lucasfcm9@gmail.com",
	"subject": "Teste",
	"text": "Hello, Java!"
}
```

É necessário configurar as seguintes variáveis dentro do `application.properties` para que o envio de e-mail funcione.

```
spring.mail.username=example@gmail.com
spring.mail.password=1234567891011123
```

É necessário que você consiga esse código de 16 caracteres na sua conta do google seguindo este tutorial:

Guia para gerar o código de 16 dígitos para configurar o SMTP do Gmail: https://support.google.com/accounts/answer/185833