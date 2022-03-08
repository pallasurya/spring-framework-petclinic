pipeline {
    agent any

    stages {

        stage("print the files") {
            steps {
                sh "pwd"
            }


        }


        stage("Delete the folder") {
            steps {
               sh "rm -rf pipeline_first"
            }
        }
         
         stage("print the folder names") {
            steps {
                sh "pwd"
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

   }
}
