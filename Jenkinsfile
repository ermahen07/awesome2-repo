pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this is my learning project'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''pwd
ls
date
cal 2023'''
          }
        }

        stage('par') {
          steps {
            echo 'learning'
            sleep(unit: 'MINUTES', time: 10)
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh '''mkdir mahi
git clone https://github.com/ermahen07/demo-jenkins.git'''
      }
    }

    stage('prod') {
      steps {
        echo 'this is last for today'
      }
    }

  }
}