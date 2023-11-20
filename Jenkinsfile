pipeline {

  agent {
     node { label 'workstation'}
   }

  stages {

      stage('Unit Tests') {
         steps {
           echo 'Unit Tests'
         }
      }

      stage('Code Analysis') {
         steps {
           sh 'sonar-scanner -Dsonar.host.url=http://172.31.83.68:9000 -Dsonar.login=admin  -Dsonar.password=admin123 -Dsonar.projectKey=frontend'
         }
      }

      stage('Security Scans') {
         steps {
            echo 'Security Scans'
         }
      }

      stage('Publish A Article') {
         steps {
           echo 'Publish A Article'
         }
      }


  }
}