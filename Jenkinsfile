pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'building app'
          }
        }

        stage('ParallelBuild') {
          steps {
            echo 'Parallel Build'
          }
        }

      }
    }

    stage('Testing') {
      steps {
        echo 'Testing now'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
      }
    }

  }
}