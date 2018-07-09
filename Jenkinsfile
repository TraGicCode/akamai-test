pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                sh 'docker run -ti -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli akamai'
            }
        }
    }
}