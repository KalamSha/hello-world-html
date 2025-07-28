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
                bat 'mkdir C:\\temp\\website'
                bat 'copy myht.html C:\\temp\\website\\'
                echo 'Deployed myht.html to C:\\temp\\website\\'
            }
        }
    }
}


