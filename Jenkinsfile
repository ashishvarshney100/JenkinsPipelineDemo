pipeline {
    agent any {}
    stages {
        stage("Git Clone") {
            steps {
                sh "Cloning git repo......."
            }
        }
        stage("Build"){
            steps {
                sh "Building code ......"
            }
        }
        stage("Test") {
            steps {
                sh "Testing code ....."
            }
        }
        stage("Deploy") {
            steps {
                sh "Deploying Code ...."
            }
        }   
    }
    post {
        success {
            echo "SUCCESS"
        }
        failure {
            echo "FAILURE"
        }
    }
}