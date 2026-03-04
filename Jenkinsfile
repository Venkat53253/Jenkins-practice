pipeline {
    agent {
        label 'agent1'
    }

    stages {
        stage ('build') {
            steps {
                echo 'building'
            }
        }
        stage ('test') {
            steps {
                echo 'testing'
            }
        }
        stage ('deploy') {
            steps {
                echo 'deploying'
            }
        }
    }
    post {
        always {
            echo 'not completed'    
        }
        success {
            echo 'sucess'
        }
        failure {
            echo 'fail'
        }
    }
}