pipeline {
    agent any
    tools{
        nodejs 'nodejs'
    }

    stages {
        stage('Checkout'){
            steps{
                   git branch : 'main', url :'https://github.com/Arvind-kumar2006/Devops1'
            }
         
        }

        stage('Build') {
            steps {
                sh 'npm run build'
                echo 'npm is create'
            }
        }
        stage('Test'){
            steps{
                sh 'npm test'
                echo 'No test defined'
            }
        }
        stage('Deploy'){
            setps{
               
                echo 'npm file runing'
            }
        }
    }
}
