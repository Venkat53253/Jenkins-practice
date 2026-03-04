pipeline {
    agent node {
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
}