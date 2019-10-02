pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
            script {
                                  powershell 'export MSYS_NO_PATHCONV=1'
                                               sh 'export MSYS_NO_PATHCONV=1'
                                                 powershell 'set MSYS_NO_PATHCONV=1'
                                                                                              sh 'set MSYS_NO_PATHCONV=1'
                                               sh 'mvn --version'
                            }

            }
        }
    }
}