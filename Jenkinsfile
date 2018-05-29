pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        sh '''echo "HELLO WORLD"
java -version

echo "${TEST_USER_USR}"
echo "${TEST_USER_PSW}"'''
      }
    }
  }
  environment {
    TEST_USER = 'credentials(\'test-user\')'
  }
}