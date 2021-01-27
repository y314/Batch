pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo %time% %date% >test123.txt'
          }
        }

        stage('') {
          steps {
            echo 'print TEST'
            build 'jobTEst'
          }
        }

      }
    }

    stage('') {
      steps {
        mail(subject: 'JenkinsTestMail', body: 'test', charset: 'utf-8', from: 'y2.71828@gmail.com', to: 'y2.71828@gmail.com')
      }
    }

  }
}