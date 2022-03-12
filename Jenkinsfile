pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Test App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'it failed', subject: 'Status of Pipeline', to: 'roy.pijush2504@gmail.com'
        }
    }
        
}
