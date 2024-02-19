docker configuration file 
pipeline {
  agent {
    docker { image 'ubuntu/apache2' }
  }
  stages {
    stage('Build') {
      steps {
         docker run -d --name apache2-container -it  -p 9999:80 ubuntu/apache2
      }
    }
  }
}
