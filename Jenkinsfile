pipeline {
    agent any

    stages {

        
         
         stage("print the folder names") {
            steps {
                sh "cd /var/lib/jenkins/workspace && ls -la"
            }


        }
        stage("checkout the code") {
            steps {
               checkout scm
            }
        }


        stage("test the code") {
            steps {
                sh "mvn clean test"
            }
        }

        stage("build the code") {
            steps {
                sh "mvn clean package"
            }


        }

        stage("print the PWD") {
            steps {
                sh "pwd"
            }


        }
        stage("print the files") {
            steps {
                sh "cd /var/lib/jenkins/workspace && ls -la"
            }


        }        
        stage("Delete the folder") {
            steps {
               sh "rm -rf /var/lib/jenkins/workspace/pipeline_first"
            }
        }
        stage("print the filfes") {
            steps {
                sh "cd /var/lib/jenkins/workspace && ls -la"
            }


        }  
   }
}
