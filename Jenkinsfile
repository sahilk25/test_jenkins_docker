pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }
    stages {
        stage('Initialize'){
            
            steps {
                def dockerHome = tool 'myDocker'
                env.PATH = "${dockerHome}/bin:${env.PATH}"
                sh 'docker --version'
            }
            
    }
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
