node {
  stage 'Checkout' {
    checkout scm
  }

  stage 'Instalar dependencias de node' {
    'npm install'
  }

  stage 'Checkout' {
    'npm run build'
  }
}
