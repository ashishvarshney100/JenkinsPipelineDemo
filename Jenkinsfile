pipeline {
    agent any 
    stages {
        stage("Git Clone") {
            steps {
                sh "Cloning git repo......."
                sh "git 'https://github.com/ashishvarshney100/JenkinsPipelineDemo.git'"
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