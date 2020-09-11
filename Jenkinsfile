pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build started...'
      }
    }

    stage('Test') {
      steps {
        echo 'Test started...'
        sleep 3
        echo 'Test finished!'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy started...'
        mail(subject: 'Finish deploy', body: 'Testing email', from: 'test-jenkins@bmw.de', to: 'intern.bmw.muc@gmail.com')
      }
    }

  }
}