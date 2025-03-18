pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('build'){
            steps{
                echo 'build app'
            }
        }
        stage('Test'){
            steps{
                echo 'Test app'
            }
        }
        stage('deploy'){
            steps{
                echo 'deploying...'
            }
        }
    }
    post{
        always{
            emailext body: 'Summary', subject: 'Pipeline Status', to:'jnkavya0@gmail.com'
        }
    }
}
