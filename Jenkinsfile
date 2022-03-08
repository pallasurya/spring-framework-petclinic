pipeline {
    agent any

    stages {
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
   }
}
