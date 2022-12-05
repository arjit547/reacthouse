pipeline {
    agent any
    stages {
        stage('git repo') {
            steps {
               
                sh "git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git"
                
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
