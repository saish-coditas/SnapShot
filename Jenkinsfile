pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sn 'npm run build' 
      }
    }
    stage('Deploy') {
      steps {
        sh 'docker build -t saishk237/snapshot-react . && docker push saishk237/snapshot-react:latest'
      }
    }
  }
}
