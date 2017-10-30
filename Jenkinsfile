pipeline {
  agent {
    node {
      label 'mod-ci-2'
    }
    
  }
  stages {
    stage('Checkout repo') {
      agent {
        docker {
          image 'modulo_ci_env'
        }
        
      }
      steps {
        sleep 1
      }
    }
  }
}