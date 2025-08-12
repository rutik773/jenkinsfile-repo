pipeline {
    agent any // Define where the pipeline will run    
    stages {
        stage('pull') { // Define a stage
            steps {
                git branch: 'main', url: 'https://github.com/iamtruptimane/Terraform-projects.git'
            }
        }
        stage('build') {
            steps {
                echo 'building...'
            }
        }
        stage('test') {
            steps {
                echo 'testing...'
            }
        }
        stage('deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }

    post { // Post-build actions
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
