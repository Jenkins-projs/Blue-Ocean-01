pipeline {
  agent any
  stages {
    stage('Stage-1') {
      steps {
        echo 'hello msg from blue ocean stage-1'
        echo 'another msg from stage-1'
      }
    }

    stage('Stage-2') {
      steps {
        writeJSON(file: 'model.json', json: 'model')
      }
    }

  }
}