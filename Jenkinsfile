pipeline {
    agent any
    stages {
        stage('Fetch Code') {
            steps {
                echo '✅ Cloning Repository...'
                bat 'git pull origin main'
            }
        }
        stage('Compile Java') {
            steps {
                echo '⚡ Compiling Java Code...'
                bat 'javac HelloWorld.java'
            }
        }
        stage('Run Java') {
            steps {
                echo '🚀 Running Java Program...'
                bat 'java HelloWorld'
            }
        }
    }
}

