pipeline {
    agent { label "linux" }
    stages {
        stage("build"){
            steps {
                sh """
                    docker build -t helloImage .
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