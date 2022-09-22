pipeline {
    agent any
    tools {
        tool name: 'Default', type: 'git'
        maven 'maven3'
    }
   stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', credentialsId: '3857d56c-4f3b-430d-b7b7-e08e21da9402', url: 'https://github.com/akandeae/Quality-life.git'
            }
        }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean'
           }
        }
    }
}
