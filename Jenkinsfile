pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli akamai'
            }
        }
    }
}