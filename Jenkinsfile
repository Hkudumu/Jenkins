pipeline {
    agent any
    environment {
      SOLUTION_NAME="Jenkin Build.sln"
	 }
    stages {
        
        stage('Build') {
            steps {
            script {
                     bat "\"${tool 'MSBuild 15.0'}\msbuild\" Jenkin Build.sln /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}
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