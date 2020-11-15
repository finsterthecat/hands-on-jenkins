pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'What\'s up doc?'
      }
    }

    stage('Test Edge') {
      parallel {
        stage('Test Edge') {
          steps {
            sh 'echo "Testing Edge"'
          }
        }

        stage('Test Chrome') {
          steps {
            sh '''echo Test fails for Chrome
exit 0
'''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy me'
      }
    }

  }
}