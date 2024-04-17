pipeline {
    agent { label 'nodes_project'}
    stages {
        stage("checkout") {
            steps {
                checkout scm 
            }
        }
        stage("Build") {
            steps {
                sh 'npm install'
            }
        }
        stage("Test") { 
            steps {
                sh 'npm test'
            }
        }
    }
}
