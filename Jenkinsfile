pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                powershell 'export MSYS_NO_PATHCONV=1'
                sh 'export MSYS_NO_PATHCONV=1'
                sh 'mvn --version'
            }
        }
    }
}