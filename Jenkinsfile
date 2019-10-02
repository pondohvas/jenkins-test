pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'export MSYS_NO_PATHCONV=1'
                sh 'mvn --version'
            }
        }
    }
}