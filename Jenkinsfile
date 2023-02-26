pipeline {
    agent {
        node{
            label "production"
        }
    }

    stages {
        stage('verify tooling') {
            steps {
                sh '''
            docker version
            docker info
            docker compose version
            curl --version
            jq --version
        '''
            }
        }
    }
}