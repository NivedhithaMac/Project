pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/NivedhithaMac/Project.git', branch: 'main', credentialsId: '947e8463-bfd5-43bc-8a66-2a35d777b537')
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t nivedhithamac/weatherapp-flask1 .'
        git(url: 'https://github.com/NivedhithaMac/Project.git', branch: 'main', credentialsId: '947e8463-bfd5-43bc-8a66-2a35d777b537')
      }
    }

  }
}