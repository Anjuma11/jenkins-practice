pipeline {

    agent {
        label "AGENT-1"
    }

    environment{
        COURSE="Jenkins"
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                    echo "building..."
            
                    env
                    """
                }
                
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