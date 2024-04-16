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
                sh 'apt install npm'
            }
        }
        stage("Test") { 
            steps {
                sh 'npm test'
            }
        }
    }
}
