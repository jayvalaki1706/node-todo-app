pipeline {
    agent any
    stages {
        stage('clone code') {
            step {
                checkout scm
            }
        }
        stage('installing npm module') {
            step {
                sh 'npm install'
            }
        }
        stage('Running the application') {
            step {
                sh 'node app.js'
            }
        }
    }
}
