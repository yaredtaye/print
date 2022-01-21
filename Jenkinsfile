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
        stage('Maven Deploy'){
            steps{
               echo " Deploying JAR file "
            }
        }
    }
}
