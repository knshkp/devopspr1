pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
            }
        }
        stage("test"){
            steps{
                sh 'brew install node'
                sh 'npm test'
            }
        }
        stage("build"){
            steps{  
                sh 'npm run build'
            }
        }   
    }
}
