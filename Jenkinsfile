pipeline {
    agent any

    stages {
        stage('Checkout'){
            git : ''
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
