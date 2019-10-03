pipeline {
    agent {
        docker {
            image 'maven:3.3.3'
         }
     }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                sh 'mvn --version'
            }
        }
    stage('Test') {
           steps {
                  sh 'mvn test'
                }
                post {
                    always {
                        junit 'target/surefire-reports/*.xml'
                    }
                }
          }
    }
}