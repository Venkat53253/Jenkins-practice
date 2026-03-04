pipeline {
    agent {
        label 'agent1'
    }

    stages {
        stage ('build') {
            steps {
                script {
                    echo 'building'
                }
            }
        }
        stage ('test') {
            steps {
                script {
                    echo 'building'
                }
            }
        }
        stage ('deploy') {
            steps {
                script {
                    echo 'building'
                }
            }
        }
    }
    
    post {
        always {
            echo 'not completed'
            deleteder()    
        }
        success {
            echo 'sucess'
        }
        failure {
            echo 'fail'
        }
    }
}