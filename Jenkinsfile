pipeline {
    agent any
    stages {
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