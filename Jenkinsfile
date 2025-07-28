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
                bat 'if not exist C:\\temp\\website mkdir C:\\temp\\website'
                bat 'copy myht.html C:\\temp\\website\\myht.html /Y'
                echo 'Deployed myht.html to C:\\temp\\website\\'
            }
        }
    }
}


