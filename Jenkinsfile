environment {
      MY_NAME = 'Mary'
      TEST_USER = credentials('test-user')
   }
pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
          echo "${TEST_USER_USR}"
          echo "${TEST_USER_PSW}"
      steps {
        cho "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
}
