pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                script {

                    docker.image('akamaiopen/cli').inside {
                        sh 'akamai promotional-deployment'
                    }
                }
            }
        }
    }
}