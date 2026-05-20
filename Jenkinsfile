pipeline {
    agent any

    tools {
        jdk 'jdk25'
    }

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/pavanreddy7-web/hello-world-java.git'
            }
        }

        stage('Compile Java Code') {
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

    post {
        success {
            echo 'Build completed successfully!'
        }

        failure {
            echo 'Build failed!'
        }
    }
}
