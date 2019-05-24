pipeline {
  agent {
    node {
      label 'master'
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