@Library("Shared") _
pipeline {
    agent {label 'vinod'}

    stages {
       stage("HELLO shared libraries NEW") {
          steps {
              print("HELLO DONE RAM")
          }  
        }
        
        stage("HELLO calling ") {
          steps {
              script {
                    print("HELLO DONE SITA")
              }
           }
        }
        stage("PRINT calling shared libraries") {
          steps {
              print("PRINT DONE RAM")
          }  
        }
        
        stage("PRINT calling ") {
          steps {
              script {
                    print("DONE SITA")
              }
           }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
        stage('create folder') {
            steps {
                sh "mkdir -p devops"
            }
        }
        
        stage('Bye') {
            steps {
                echo 'Bye my friends'
            }
        }
    }
}
