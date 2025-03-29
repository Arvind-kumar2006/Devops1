pipeline {
    agent any
    tools{
        Nodejs 'Nodejs'
    }

    stages {
        stage('Checkout'){
            git branch 'main', url :'https://github.com/Arvind-kumar2006/Devops1'
        }

        stage('Build') {
            steps {
                sh 'npm run build'
                echo 'npm is create'
            }
        }stage('Test'){
            steps{
                sh 'npm test'
                echo 'No test defined'
            }
        }stage('Deploy'){
            setps{
                sh 'npm run dev'
                echo 'npm file runing'
            }
        }
    }
}
