#!groovy
pipeline {
 

    agent {
           label 'ubuntu1604'
      }

      stages {
           stage('Simulated deploy') {
                when { branch 'jervis_simple' }
                steps {
                    sh 'env | LC_ALL=C sort'
                    unstash 'artifacts'
                    unstash 'junit'
                    sh 'find . -type f'
          }
       }
    }
}
