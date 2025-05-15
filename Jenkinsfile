pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }

        stage('Complete') {
            steps {
                echo 'Completed...'
            }
        }
    }

    post {
        success {
            mail to: 'simashakavindi@gmail.com',
                 subject: 'Build Status Email',
                 body: 'Build was successful'
        }
    }
}
