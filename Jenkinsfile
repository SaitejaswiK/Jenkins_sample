pipeline{
    agent any
    
    environment{
        PATH = "C:\Users\Koppu\Downloads\apache-maven-3.6.0\bin:$PATH"
    }
    stages{
        stage("Git Checkout"){
            steps{
                git 'https://github.com/SaitejaswiK/Jenkins_sample/'
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn clean package"
            }
        }
}
