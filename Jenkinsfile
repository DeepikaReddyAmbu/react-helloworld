pipeline {
    agent any
    tools {nodejs "nodejs"}
    stages {
        stage("checkout") {
            steps {
                checkout scm
            }
        }
    stages {
        stage('Example') {
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
