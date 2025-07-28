pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the repository...'
                checkout scm
            }
        }

        stage('Deploy') {
            steps {
                echo 'Simulating deployment...'
                sh 'mkdir -p /tmp/website'
                sh 'cp index.html /tmp/website/'
                echo 'Deployed index.html to /tmp/website/'
            }
        }
    }
}


