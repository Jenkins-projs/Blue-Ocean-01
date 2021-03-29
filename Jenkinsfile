pipeline {
  agent any
  stages {
    stage('Stage-1') {
      steps {
        echo 'hello msg from blue ocean stage-1 edited from git'
        echo 'another msg from stage-1'
      }
    }

    stage('Stage-2') {
      steps {
        echo 'from stage-2'
      }
    }

    stage('stage 3') {
      steps {
        input(message: 'Do you want to continue ?', id: '1', ok: '2', submitter: '3', submitterParameter: '4')
      }
    }

  }
}