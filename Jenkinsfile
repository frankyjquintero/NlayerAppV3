pipeline {
  agent {
    node {
      label 'Node1'
    }

  }
  stages {
    stage('') {
      steps {
        withSonarQubeEnv('sonar') {
          waitForQualityGate true
          bat(script: 'bat', returnStatus: true, returnStdout: true)
          error 'khe'
        }

      }
    }
  }
}