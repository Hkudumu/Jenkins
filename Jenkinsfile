pipeline {
    agent any

    stages {
        
        stage('Build') {
            steps {
                      bat "${msbuild}/msbuild  ${SOLUTION_NAME}"

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}