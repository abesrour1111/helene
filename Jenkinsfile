pipeline {
  agent any
  stages {
    stage('job1') {
      parallel {
        stage('job1') {
          steps {
            sh '''date


'''
          }
        }

        stage('job1bis') {
          steps {
            sh 'dpkg -l > /tmp/paquets'
          }
        }

      }
    }

    stage('job2') {
      steps {
        sh 'cut -d\':\' -f1,3 /etc/passwd > /tmp/users'
      }
    }

  }
}