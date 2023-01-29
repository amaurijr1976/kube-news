pipeline{
    agent any
    stages {

        stage ('Build Docker Image'){
            steps{
                script{
                    dockerapp= docker.Build("amaurijr1976/kube-news:${env:BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}