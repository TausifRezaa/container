pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'Building' 
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploying'
                sh'exit'
                sh'pwd'
                sh'docker exec -u 0 -it laravel-app /bin/bash'
                sh'git pull origin master'
            }
        }
    }
}
