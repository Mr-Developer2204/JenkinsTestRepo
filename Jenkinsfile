pipeline{
    agent any
    stages{
        stage('Pull')
        {
            steps{
                bat 'git pull origin main'
            }
        }
        stage('Build')
        {
            //Steps to build a react app in windows
            steps{
                echo 'Building React App'
                bat 'npm install'
                bat 'npm run build'
            }
        }
        stage('Deploy')
        {
            steps{
                bat 'npm start'
            }
        }
    }
}
