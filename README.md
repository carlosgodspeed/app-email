# App de E-mail em PHP

Este é um aplicativo simples em PHP que permite enviar e-mails através de um formulário. O aplicativo utiliza a biblioteca PHPMailer para facilitar o envio de e-mails por meio do servidor SMTP do Gmail. 

<strong>Desenvolvido durante o curso  de Desenvolvimento Web na Plataforma da Udemy.</strong>

## Requisitos

Antes de utilizar o aplicativo, certifique-se de ter o seguinte:

- Servidor web com suporte para PHP.
- Biblioteca PHPMailer configurada corretamente no diretório `./bibliotecas/PHPMailer/`.

## Configuração

Siga as etapas abaixo para configurar o aplicativo:

1. Faça o download da biblioteca PHPMailer em [https://github.com/PHPMailer/PHPMailer](https://github.com/PHPMailer/PHPMailer) e extraia os arquivos para o diretório `./bibliotecas/PHPMailer/` no seu servidor web.

2. Abra o arquivo PHP do seu aplicativo em um editor de texto.

3. Na seção "Server settings", você precisa configurar as informações de autenticação do servidor SMTP para enviar e-mails através do Gmail. Certifique-se de preencher corretamente os seguintes campos:
   
   - `$mail->Host`: Insira o host do servidor SMTP do Gmail (geralmente é 'smtp.gmail.com').
   - `$mail->SMTPAuth`: Defina como `true` para habilitar a autenticação SMTP.
   - `$mail->Username`: Insira o endereço de e-mail do remetente.
   - `$mail->Password`: Insira a senha do remetente.
   - `$mail->SMTPSecure`: Defina como `PHPMailer::ENCRYPTION_STARTTLS`.
   - `$mail->Port`: Defina a porta do servidor SMTP do Gmail (geralmente é 587).

4. Salve o arquivo após fazer as alterações.

## Uso

Após configurar o aplicativo, você pode acessá-lo abrindo o navegador e digitando o endereço do seu servidor web.

O aplicativo apresentará um formulário contendo os campos "Para", "Assunto" e "Mensagem". Preencha esses campos corretamente e clique no botão "Enviar" para enviar o e-mail.

O aplicativo irá validar os campos e, se todos estiverem preenchidos corretamente, tentará enviar o e-mail. Se o envio for bem-sucedido, você verá uma mensagem de sucesso. Caso ocorra algum erro, você verá uma mensagem de erro detalhando o problema encontrado.

## Limitações

Este aplicativo possui algumas limitações:

- Ele foi projetado para enviar e-mails apenas através do servidor SMTP do Gmail. Se você deseja utilizar outro servidor SMTP, será necessário modificar as configurações do aplicativo.
- Não há suporte para anexos de arquivos.
- Não há recursos avançados de formatação de e-mail (apenas texto simples).

![Captura de Tela (27)](https://github.com/carlosgodspeed/app-email/assets/100007663/7293bd09-dbe2-4bf7-9724-8c1938ae83a9)
