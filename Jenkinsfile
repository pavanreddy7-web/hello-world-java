// pipeline {
//     agent any

//     tools {
//         jdk 'JDK17'
//     }

//     stages {

//         stage('Clone Repository') {
//             steps {
//                 git 'https://github.com/pavanreddy7-web/hello-world-java'
//             }
//         }

//         stage('Compile Java Code') {
//             steps {
//                 sh 'javac HelloWorld.java'
//             }
//         }

//         stage('Run Java Program') {
//             steps {
//                 sh 'java HelloWorld'
//             }
//         }
//     }

//     post {
//         success {
//             echo 'Build completed successfully!'
//         }

//         failure {
//             echo 'Build failed!'
//         }
//     }
// }



pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}





