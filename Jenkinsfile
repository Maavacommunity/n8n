pipeline {
    agent any

    environment {
        DEPLOYMENT_NAME = 'n8n'
        DEPLOYMENT_DOMAIN = 'n8n.maava.org'
        DEPLOYMENT_PORT = '5678'  // Optional
    }

    stages {
        stage('Deployment') {
            steps {
                sh '''
                    export DEPLOYMENT_NAME=${DEPLOYMENT_NAME}
                    export DEPLOYMENT_DOMAIN=${DEPLOYMENT_DOMAIN}
                    export DEPLOYMENT_PORT=${DEPLOYMENT_PORT}

                    DEPLOYMENT
                '''
            }
        }
    }
}
