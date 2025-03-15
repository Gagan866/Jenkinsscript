pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    echo 'Cloning Repository...'
                }
            }
        }
        stage('Compile Java') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }
        stage('Run Java Program') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}
