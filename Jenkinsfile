node {
  stage 'Checkout' {
    checkout scm
  }

  stage 'Instalar dependencias de node' {
    'npm install'
  }

  stage 'Constuir' {
    'npm run build'
  }
}
