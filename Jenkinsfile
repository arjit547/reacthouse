pipeline {
    agent any
    stages {
        stage('git repo') {
            steps {
               
                sh "git clone https://github.com/arjit547/reacthouse.git"
                cd reacthouse
                npm install
                npm run build
                npm start
            }
        }
        
    }
}
