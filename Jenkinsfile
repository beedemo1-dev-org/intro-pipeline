environment {
      MY_NAME = 'Mary'
      TEST_USER = credentials('test-user')
   }
parameters {
      string(name: 'Name', defaultValue: 'whoever you are', 
	     description: 'Who should I say hi to?')
   }
pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
          echo "${TEST_USER_USR}"
          echo "${TEST_USER_PSW}"
    }
      steps {
        echo "Hello ${params.Name}!"
        sh 'java -version'
      }
    }
  }

