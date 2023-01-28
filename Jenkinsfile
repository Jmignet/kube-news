pipeline {
    agent any

    stages {
        
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("jmignet/kube-news:${env.BUILD_ID}", "-f ./src/dockerfile ./src")
                }
            }
        }
        
    }

}