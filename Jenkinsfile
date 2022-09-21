pipeline {
    agent any
    tools {
        tools {
  maven 'maven3'
}
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', credentialsId: '3857d56c-4f3b-430d-b7b7-e08e21da9402', url: 'https://github.com/bloomytech/samplemaven.git'
            }
        }
    stages {
        stage('Build') {
            steps {
                sh '''mvn clean install ''' 
            }
        }
    }
}
}
