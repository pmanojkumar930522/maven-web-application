pipeline{
    agent any
    tools {
     maven 'maven-latest'
    }
    stages{
        stage('Git Checkout'){
            steps{
                echo "Gettig details from git"
                git credentialsId: '36f3f88d-e209-47eb-9383-80c6f48983f1', url: 'https://github.com/pmanojkumar930522/maven-web-application.git' 
            }
        }
        stage('Build'){
            steps{
                echo "Build using maven"
                sh "mvn clean package"
                
            }
        }
    }
}
