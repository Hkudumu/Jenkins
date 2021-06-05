pipeline {
    agent any
    environment {
      SOLUTION_NAME="Jenkin Build.sln"
	 }
    stages {
        
        stage('Build') {
            steps {
            script {
                     bat 'dotnet build Jenkin Build\\Jenkin Build.Sln'
                     }

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}