pipeline {
    agent any
    environment {
      SOLUTION_NAME="CAPSService2.0.sln"
	 }
    stages {
        
        stage('Build') {
            steps {
            script {
                     def msbuild = tool name: 'MSBuild v1'
                      bat "${msbuild}/msbuild  ${SOLUTION_NAME}"
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