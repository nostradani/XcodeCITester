pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        parallel(
          "Test": {
            echo 'Build 1'
            echo 'Build2'
            
          },
          "Build 2": {
            echo 'Build 2'
            
          }
        )
      }
    }
    stage('Upload') {
      steps {
        parallel(
          "Upload1": {
            echo 'Upload'
            
          },
          "Upload2": {
            echo 'Upload 2'
            
          }
        )
      }
    }
    stage('Finish') {
      steps {
        echo 'Finish'
      }
    }
  }
}