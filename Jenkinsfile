pipeline {
    agent {
        docker {
            image 'akamaiopen/cli'
            args '--entrypoint=""'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                sh 'ls -la'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli install promotional-deployment'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli promotional-deployment'
            }
        }
    }
}