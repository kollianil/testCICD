pipeline {
  agent any
  stages {
    stage('CODE') {
      steps {
        sh 'echo \'Welcome to my pipeline\''
      }
    }

    stage('Compile') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('Package') {
      steps {
        sh 'mvn package'
      }
    }

    stage('Deploy') {
      steps {
        sh 'java -jar target/'
      }
    }

    stage('End') {
      steps {
        sh 'echo "pipeline sucesssssssss"'
      }
    }

  }
}