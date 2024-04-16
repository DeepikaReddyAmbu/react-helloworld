pipeline {
    agent any
    stages {
        stage("checkout") {
            steps {
                checkout scm 
            }
        }
        stage("Build") {
            steps {
                sh 'apt-get install -y npm'
            }
        }
        stage("Test") { 
            steps {
                sh 'npm test'
            }
        }
    }
}
