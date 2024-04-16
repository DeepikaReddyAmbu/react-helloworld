pipeline {
    agent any
    tools {nodejs "nodejs"}
    stages {
        stage("checkout") {
            steps {
                checkout scm 
            }
        }
        stage("Example") { 
            steps {
                sh 'npm config ls'
            }
        }
        stage("Test") {
            steps {
                sh 'npm install'
            }
        }
        stage("Build") { 
            steps {
                sh 'npm run build'
            }
        }
    }
}
