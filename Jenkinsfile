pipeline {
  agent any
  stages {
    stage('re-Build') {
      steps {
        echo 'Building !!!'
      }
    }
    stage('Test') {
      parallel {
        stage('PCC Test') {
          steps {
            sleep 3
            echo 'PCC Tests over!'
          }
        }
        stage('Susan Tests') {
          steps {
            sleep 2
            echo 'Susan Tests Over!'
          }
        }
      }
    }
    stage('Deploy!') {
      steps {
        echo 'Deploy!'
      }
    }
  }
}