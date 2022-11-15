pipeline{
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages{
        stage('Git checkout'){
            steps{
                script{
                    git branch: 'main', url: 'https://github.com/Chanti369/demoapp.git'
                }
            }    
        }
        stage('Unit Testing'){
            steps{
                sh 'mvn test'
            }
        }
    }
}
