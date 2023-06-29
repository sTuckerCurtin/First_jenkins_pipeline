
pipeline {
  agent any

  stages {

    stage('Build') {
      steps {
        sh 'echo "Building the application..."'
      }
    }

    stage('Docker') {
  steps {
    withCredentials([usernamePassword(credentialsID: 'personal-docker-credentials', usernameVariable: 'DOCKER_USERNAME', passwordVariable: 'DOCKER_PASSWORD')]){
      sh "echo \$DOCKER_USERNAME"
    }
  }
}

  }
}
