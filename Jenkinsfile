environment {
      MY_NAME = 'Mary'
   }
pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      steps {
        cho "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
}
