pipeline {
    agent any
    stages {
        stage("checkout") {
            steps {
                checkout scm 
            }
        }
    tools {nodejs "nodejs"}
        stage("Example") { 
            steps {
                sh 'npm config ls'
            }
        }
        stage("Test") {
            steps {
                sh 'npm install'
                sh 'npm test'
            }
        }
        stage("Build") { 
            steps {
                sh 'npm run build'
            }
        }
    }
}
