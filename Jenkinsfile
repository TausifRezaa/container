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
                sh'git pull origin master'
            }
        }
    }
}
