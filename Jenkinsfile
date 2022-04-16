pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout'
      }
    }

    stage('Deployment') {
      when {
        expression {
          env.GIT_BRANCH == 'master'
        }

      }
      steps {
        echo 'Deployement'
        sh '''
        rm -rf /var/www/html/jasonhaenlin/*;


      

mv * /var/www/html/jasonhaenlin/
        '''
      }
    }

  }
  post {
    always {
      echo 'JENKINS PIPELINE'
    }

    success {
      echo 'JENKINS PIPELINE SUCCESSFUL'
    }

    failure {
      echo 'JENKINS PIPELINE FAILED'
    }

    unstable {
      echo 'JENKINS PIPELINE WAS MARKED AS UNSTABLE'
    }

    changed {
      echo 'JENKINS PIPELINE STATUS HAS CHANGED SINCE LAST EXECUTION'
    }

  }
  options {
    disableConcurrentBuilds()
    timeout(time: 1, unit: 'HOURS')
  }
}