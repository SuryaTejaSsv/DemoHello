pipeline {
    agent any
    stages {
         stage("initial"){
            steps {
                sh """
                    docker --version
                """
            }
        }
        stage("build"){
            steps {
                sh """
                    docker build -t helloimage .
                """
            }
        }
        stage("run") {
            steps {
                sh """
                    docker compose up
                """
            }
        }
    }
}