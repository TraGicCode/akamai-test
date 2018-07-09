pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                script {

                    docker.image('akamaiopen/cli') {
                        sh 'akamai promotional-deployment'
                    }
                }
            }
        }
    }
}