pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello from the trigger'
      }
    }

    stage('outfile') {
      steps {
        sh 'echo "helloworld" >> blueocean'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}