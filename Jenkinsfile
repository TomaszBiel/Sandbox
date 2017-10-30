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
        git(credentialsId: 's3-firmwareFullAccess', branch: '\'*/SS-691_test1\'', url: '\'https://github.com/homersoft/FW-MODULO-CI.git\'')
      }
    }
  }
}