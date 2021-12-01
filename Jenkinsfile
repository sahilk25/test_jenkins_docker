pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }
    stages {
        stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
