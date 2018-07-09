pipeline {
    agent {
        docker {
            image 'akamaiopen/cli'
        }
    }

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                sh 'pwd'
            }
        }
    }
}