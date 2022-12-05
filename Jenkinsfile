pipeline {
    agent any
    stages {
        stage('git repo') {
            steps {
               
                bat "git clone https://github.com/arjit547/reacthouse.git"
                
            }
        }
        stage('install') {
            steps {
                bat "npm install"
            }
        }
        stage('build') {
            steps {
                bat "npm run build"
            }
        }
        stage('start') {
            steps {
                bat "npm start"
            }
        }
    }
}