pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('compile') {
      steps {
        sh './gradlew assembleDebug'
      }
    }
    stage('Test') {
      steps {
        sh './gradlew testDebugUnitTest testDebugUnitTest'
      }
    }
  }
}