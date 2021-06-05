pipeline {
    agent any

    stages {
        
        stage('Build') {
            steps {
            script {
                     def msbuild = tool name: 'MSBuild v4.0.30319'
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