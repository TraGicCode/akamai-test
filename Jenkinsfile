pipeline {
    agent {
        docker {
            image 'akamaiopen/cli'
            args '--entrypoint="cat"'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                sh 'docker exec akamai help'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli install promotional-deployment'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli promotional-deployment'
            }
        }
    }
}