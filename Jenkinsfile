pipeline {
    agent {
        docker {
            image 'maven:3.3.3'
            args '-w C:\\Users\\teste\\.jenkins\\workspace\\Java_maven_master'
         }
     }
    stages {
        stage('build') {
            steps {
                bat 'set'
                sh 'echo "Hello World"'
                sh 'docker run --help'
                sh 'export MSYS_NO_PATHCONV=1'
                sh 'mvn --version'
            }
        }
    }
}