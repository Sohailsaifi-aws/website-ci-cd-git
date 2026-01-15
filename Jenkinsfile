pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Sohailsaifi-aws/website-ci-cd-git.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build started'
                sh 'ls'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying website'
                sh 'sudo cp -r startbootstrap-agency-master/* /var/www/html/'
            }
        }
    }
}
