pipeline {
    agent any
    stages {
        stage('git repo') {
            steps {
               
                sh "git clone https://github.com/arjit547/reacthouse.git"
                
            }
        }
        stage('Build') {
            steps {
                sh "npm install"
                sh "npm run build"
            }
        }
        
    }
}
