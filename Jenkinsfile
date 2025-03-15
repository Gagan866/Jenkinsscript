pipeline {
    agent any

    environment {
        JAVA_HOME = "C:\\Program Files\\Java\\jdk-21"
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }

    stages {
        stage('Clone Repository') {
            steps {
                script {
                    echo 'Fetching latest code from GitHub...'
                    checkout scm
                }
            }
        }

        stage('Compile Java Code') {
            steps {
                script {
                    echo 'Compiling Java File...'
                    bat 'javac HelloWorld.java'
                }
            }
        }

        stage('Run Java Program') {
            steps {
                script {
                    echo 'Running Java Program...'
                    bat 'java HelloWorld'
                }
            }
        }
    }
}
