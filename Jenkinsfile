pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                sh 'akamai promotional-deployment'

                docker.image('akamaiopen/cli') {
                    sh 'akamai promotional-deployment'
                }
            }
        }
    }
}