pipeline{
    agent any
    stages{
        stage("Git"){
            steps{
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/SourabhCG0613/maven.git'
            }
        }
        stage("Maven"){
            steps{
                sh "mvn clean package"
            }
        }
    }
}
