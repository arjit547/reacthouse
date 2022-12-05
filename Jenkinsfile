pipeline {
    agent any
    stages {
        stage('git repo') {
            steps {
               
                sh "git clone https://github.com/arjit547/reacthouse.git"
                
            }
        }
        stage('install') {
            steps {
                sh "npm install"
            }
        }
        stage('build') {
            steps {
                sh "npm run build"
            }
        }
        stage('start') {
            steps {
                sh "npm start"
            }
        }
    }
}
