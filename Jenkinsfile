pipeline {
  agent any
  stages {
    stage('Githubcheckout') {
      parallel {
        stage('Githubcheckout') {
          steps {
            git(url: 'https://github.com/sarthak1007/Java-Hello', branch: 'master')
          }
        }

        stage('build') {
          steps {
            input(message: 'okay', ok: 'do it')
          }
        }

        stage('deploy') {
          steps {
            sh 'echo "It is deployed"'
          }
        }

      }
    }

  }
}