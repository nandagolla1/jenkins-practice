pipeline {
    agent {
        label 'Agent-1'
    }

    // build
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    // post build
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'hello success!'
        }
        failure { 
            echo 'hello failure!'
        }
    }

}