pipeline {
    agent any

    stages {
        stage('Deploy - Staging Environment (EPN)') {
            steps {
                echo 'Deploying to Staging Environment'
                script {

                    docker.image('akamaiopen/cli').withRun('-e "MYSQL_ROOT_PASSWORD=my-secret-pw"') {
                        sh 'pwd'
                    }
                }
            }
        }
    }
}