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
    bat 'C:\\Users\\Lyrus\\AppData\\Local\\Programs\\Python\\Python312\\python.exe C:\\Users\\Lyrus\\Documents\\Prog\\mail.py'
  }
}
