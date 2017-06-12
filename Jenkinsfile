pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        echo 'BUILD_STEP_1'
      }
    }
    stage('BUILD_CHANEL') {
      steps {
        sleep(time: 5, unit: 'SECONDS')
      }
    }
    stage('BUILD_FINAL') {
      steps {
        echo 'final'
      }
    }
    stage('DEPLOY') {
      steps {
        retry(count: 4) {
          retry(count: 2)
        }
        
      }
    }
  }
}