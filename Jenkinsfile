pipeline {
    agent {
        docker {
            image 'akamaiopen/cli'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                sh 'install promotional-deployment'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli install promotional-deployment'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli promotional-deployment'
            }
        }
    }
}