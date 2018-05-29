pipeline {
  agent any
  stages {
    stage('step1') {
      agent any
      steps {
        sh '''echo "HELLO WORLD"
java -version'''
      }
    }
    stage('Deploy') {
      steps {
        input(message: 'should we continue?', id: 'non', ok: 'yes ')
      }
    }
  }
}