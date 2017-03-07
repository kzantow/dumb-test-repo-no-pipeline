pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
        sh 'echo \'hello\'\'! #$%#$%  " @#$@3'
        echo 'yikes\' \'dasf "EW #$%#@$% ""'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Chrome": {
            echo 'testing in chrome'
            
          },
          "Firefox": {
            echo 'testing in firefox'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'deploying'
      }
    }
  }
  environment {
    asdf = '\''
  }
}