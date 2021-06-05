pipeline {
    agent any

    stages {
        
        stage('Test') {
            steps {
                      bat "dotnet restore YourProjectPath\\Your_Project.csproj"

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}