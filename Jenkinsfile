pipeline {
    agent {
        label 'agent1'
    }
    enviornment {
        course = 'jenkins'
    }
    options {
        timeout(time: 30, unit: 'MINUTES') 
        disableConcurrentBuilds()

    stages {
        stage ('build') {
            steps {
                script {
                    sh """
                       echo "hello build"
                       env
                    """
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