pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('test') {
      steps {
        echo 'testing'
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            echo 'testing'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploying'
          }
        }

        stage('operate') {
          steps {
            echo 'operating'
          }
        }

      }
    }

  }
}