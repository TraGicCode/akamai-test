pipeline {
    agent {
        docker {
            image 'akamaiopen/cli'
            // https://github.com/jenkinsci/docker-workflow-plugin/pull/116
            // args '--entrypoint=""'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                sh '/usr/local/bin/akamai'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli install promotional-deployment'
                //sh 'docker run -i -v $HOME/.edgerc:/root/.edgerc akamaiopen/cli promotional-deployment'
            }
        }
    }
}