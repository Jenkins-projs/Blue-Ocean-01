pipeline {
  agent any
  stages {
    stage('Stage-1') {
      parallel {
        stage('Stage-1') {
          steps {
            echo 'hello msg from blue ocean stage-1 edited from git'
            echo 'another msg from stage-1'
          }
        }

        stage('stage1-1') {
          steps {
            echo 'stage 1-1'
          }
        }

        stage('stage 1-2') {
          steps {
            echo 'stage1-2'
          }
        }

      }
    }

    stage('Stage-2') {
      parallel {
        stage('Stage-2') {
          steps {
            echo 'from stage-2'
          }
        }

        stage('stage 2 -1') {
          steps {
            echo 'stage 2-1'
          }
        }

        stage('stage 2-2') {
          steps {
            echo 'stage 2-2'
          }
        }

      }
    }

    stage('stage 3') {
      parallel {
        stage('stage 3') {
          steps {
            input(message: 'Do you want to continue ?', id: '1', submitter: '3', submitterParameter: '4')
          }
        }

        stage('stage 3-1') {
          steps {
            echo 'stage 3-1'
          }
        }

        stage('stage 3-2') {
          steps {
            echo 'stage 3-2'
          }
        }

        stage('stage -3-3') {
          steps {
            echo 'stage 3-3'
          }
        }

        stage('stage-3-5') {
          steps {
            echo 'one more msg'
          }
        }

        stage('stage 3 - 6') {
          steps {
            echo 'hi'
          }
        }

      }
    }

  }
}