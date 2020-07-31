pipeline{
    agent any
    
    environment{
        PATH = "C:\Users\Koppu\Downloads\apache-maven-3.6.0\bin:$PATH"
    }
    stages{
        stage("Git Checkout"){
            steps{
                git credentialsId: 'github', url: 'https://github.com/javahometech/myweb'
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn clean package"
            }
        }
}
