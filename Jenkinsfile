pipeline {
    agent any

    stages {
        
        stage('Restore') {
            steps {
                      bat "dotnet restore ${workspace}\\Jenkin Build.csproj"

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}