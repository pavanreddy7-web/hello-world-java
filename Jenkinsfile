pipeline {
    agent any

    tools {
        jdk 'JDK25'
    }

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/pavanreddy7-web/hello-world-java'
            }
        }

        stage('Compile Java Code') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run Java Program') {
            steps {
                sh 'java HelloWorld'
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







