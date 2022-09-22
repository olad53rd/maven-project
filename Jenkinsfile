pipeline {
    agent any
    tools {
        tool name: 'Default', type: 'git'
        maven 'maven3'
    }
    stages {
        stage('SCM Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/bloomytech/samplemaven.git']]])
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
