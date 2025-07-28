pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the repository...'
                checkout scm
            }
        }

        stage('Build C Program') {
            steps {
                echo 'Compiling hello.c...'
                bat 'gcc hello.c -o hello.exe'
            }
        }

        stage('Run') {
            steps {
                echo 'Running program...'
                bat '.\\hello.exe'
            }
        }
    }
}
