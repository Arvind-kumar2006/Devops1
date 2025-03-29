pipeline{
    agent any

    stages{
        stage('Checkout'){
            steps{
             git : 'https://github.com/Arvind-kumar2006/Evaluation',branch :'main'
            }
            stage('Build'){
                steps{
                    sh 'npm run build'
                }
            }stage('Test'){
                steps{
                    sh 'npm test'
                    echo 'No tests defined'
                }
            }
            stage('Deploy'){
                steps{
                sh 'npm run dev'
                }
            }
        }
    }
}