pipeline {
    agent {
        label 'Agent-1'
    }
    environment { 
        COURSE = 'jenkins'
    }

    // build
    stages {
        stage('Build') {
            steps {
                script{
                    echo 'Building..'
                }
            }
        }
        stage('Test') {
            steps {
                script{
                    echo 'Testing..'
                }
            }
        }
        stage('Deploy') {
            steps {
                script{
                    echo 'Deploying....'
                }
            }
        }
    }
    // post build
    post { 
        always { 
            echo 'I will always say Hello again!'
            deleteDir()
        }
        success { 
            echo 'hello success!'
        }
        failure { 
            echo 'hello failure!'
        }
    }

}