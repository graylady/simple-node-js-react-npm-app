pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build Production files') {
            steps {
                bat 'npm run build'
            }
        }
       stage('test') {
            steps {
                bat 'npm run test'
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}