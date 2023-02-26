pipeline {
    agemt {
        node {
            label "production"
        }
    }

    stages {
        stage("verify tooling"){
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