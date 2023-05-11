pipeline{
  agent {
    label "jenkins-agent"
  }
  tools {
    jdk 'Java17'
    maven 'Maven3'
  }
  stages {
    stage("Clean Workspace") {
      steps{
        cleanWs()
      }
    }

    stage("Checkout from SCM") {
      steps{
        git branch: 'main', credentialsID: 'github', url: 'https://github.com/nulldoot2k/complete-prodcution-e2e-pipeline'
      }
    }
  }
}
