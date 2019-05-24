pipeline {
  agent {
    node {
      label 'android'
    }

  }
  stages {
    stage('compile') {
      steps {
        sh './gradlew compileDebugSources'
      }
    }
    stage('Test') {
      steps {
        sh './gradlew testDebugUnitTest testDebugUnitTest'
      }
    }
  }
}