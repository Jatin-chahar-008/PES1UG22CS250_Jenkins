pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ your_code.cpp -o PES1UG22CS250-1'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG22CS250-1'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
