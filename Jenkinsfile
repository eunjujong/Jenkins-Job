pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building App'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying App'
            }
        }
    }
    post {
        failure {
            emailext body: 'Summary', subject: 'Pipeline Stratus', to: 'eunjujong95@gmail.com'
        }
    }
}
