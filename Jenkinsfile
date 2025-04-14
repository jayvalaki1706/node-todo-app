pipeline {
    agent any
    stages {
        stage('clone code') {
            steps {
                checkout scm
            }
        }
        stage('installing npm module') {
            steps {
                sh 'npm install'
                sh 'npm --version'
            }
        }
        stage('Running the application') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
