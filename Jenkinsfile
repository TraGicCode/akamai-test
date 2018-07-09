pipeline {
    agent {
        docker {
            image 'docker pull akamaiopen/cli'
            args '-p 3000:3000'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                sh 'akamai promotional-deployment'
            }
        }
    }
}