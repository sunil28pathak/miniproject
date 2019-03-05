pipeline {
  agent any
  stages {
    stage('') {
      steps {
        bat 'findstr /N /C:"************Policy Center Ready************" output\\\\usefulfile.txt'
        timeout(time: 6, activity: true) {
          retry(count: 4) {
            echo 'Success'
          }

        }

      }
    }
  }
}