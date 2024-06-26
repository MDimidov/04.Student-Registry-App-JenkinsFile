pipeline{
    agent any
    stages{
        stage("NPM Install"){
            steps{
                bat 'npm install'
            }
        }
        stage("NPM Audit"){
            steps{
                bat 'npm audit fix --force'
            }
        }
        stage("Run integration tests"){
            steps{
                bat 'npm test'
            }
        }
    }
}