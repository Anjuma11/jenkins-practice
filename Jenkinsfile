pipeline {
    agent any{
        label "AGENT-1"
    }
    stages {
        stage('Build') {
            steps {
                echo "building..."
            }
        }
        stage('Test') {
            steps {
                echo "testing..."
            }
        }
        stage('Deploy') {
            steps {
                echo "deploying..."
            }
        }
    }
    
    post{
        always{
            echo "I will always say hello again"
            deleteDir()
        }
        success{
            echo "Hello Success..."
        }
        failure{
            echo "Hello Failure..."
        }

    }
}