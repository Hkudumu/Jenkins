pipeline {
    agent any

    stages {
        
        stage('Restore') {
            steps {
                      bat "dotnet restore ${workspace}"

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}