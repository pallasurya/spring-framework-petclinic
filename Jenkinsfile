pipeline {
    agent any

    stages {
         
        stage("checkout the code") {
            steps {
               checkout scm
            }
        }

        stage("Delete the folder") {
            steps {
               sh "rm -rf pipeline_first"
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
