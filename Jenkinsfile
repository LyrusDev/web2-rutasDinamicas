node {
  stage('Checkout') {
    checkout scm
  }

  stage('Instalar dependencias de node') {
    'npm install'
  }

  stage('Constuir') {
    'npm run build'
  }
}

import smtplib
from email.mime.text import MIMEText
from email.mime.multipart import MIMEMultipart

def enviar_correo(destinatario, asunto, mensaje, remitente, contraseña, servidor_smtp, puerto_smtp):
    # Configuración del mensaje
    msg = MIMEMultipart()
    msg['From'] = remitente
    msg['To'] = destinatario
    msg['Subject'] = asunto

    # Añadir el cuerpo del mensaje
    msg.attach(MIMEText(mensaje, 'plain'))

    # Establecer conexión al servidor SMTP
    try:
        server = smtplib.SMTP(host=servidor_smtp, port=puerto_smtp)
        server.starttls()
        server.login(remitente, contraseña)

        # Enviar el mensaje
        server.sendmail(remitente, destinatario, msg.as_string())
        print("Correo enviado exitosamente")

    except Exception as e:
        print(f"Error al enviar el correo: {str(e)}")

    finally:
        # Cerrar la conexión al servidor SMTP
        server.quit()

# Ejemplo de uso
if __name__ == "__main__":
    destinatario = "prueba-mail@yopmail.com"
    asunto = "¡Hola desde Python!"
    mensaje = "Este es un correo de prueba enviado desde un script de Python."
    remitente = "aldoguizado11@gmail.com"
    contraseña = "yasj emep yuvh yiss"
    servidor_smtp = "smtp.gmail.com"
    puerto_smtp = 587

    enviar_correo(destinatario, asunto, mensaje, remitente, contraseña, servidor_smtp, puerto_smtp)
