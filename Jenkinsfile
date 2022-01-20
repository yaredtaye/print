pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "building print service"'
      }
    }

    stage('Test') {
      steps {
        sh 'echo "testing print dervice"'
      }
    }

    stage('Deploy to staging') {
      steps {
        sh 'echo "Deploy print service staging"'
      }
    }
    stage('Deploy to prod') {
      steps {
        sh 'echo "Deploy print service to production"'
      }
    }

  }
}
