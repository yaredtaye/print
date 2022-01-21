pipeline{
    agent any
    stages {
        stage('Git Clone'){
            steps{
                git credentialsId: '44a5733f-4a10-4f32-b366-84adf96d94da', url: 'https://github.com/yaredtaye/print.git'
            }
        }
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Build Docker Image'){
            steps{
               sh "docker build -t fayda/print:1.1.4 ."
            }
        }
        stage('Deploy docker to Staging'){
            steps{
               echo " Deploying Docker to staging area "
            }
        }
    }
}
