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

  stage('Ejecutar script Python') {
    sh 'python C:\\Users\\Lyrus\\Documents\\Prog\\mail.py'
  }
}
