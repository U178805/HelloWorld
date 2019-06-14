pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
            args '-u root:sudo -v /var/lib/jenkins/workspace/JenkinsFile:/JenkinsFile'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
