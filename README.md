pipeline {
    agent any
    stages {
        stage('welcome step') {
            steps {
               slackSend channel: 'tech_team', message: 'This is test message'
            }
        }
    }
}

