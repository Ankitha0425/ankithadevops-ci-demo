pipeline {
    agent {
        label 'agent1'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Build is running on agent1'
                sh 'echo Running on: $(hostname)'
                sh 'java -version'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing on agent1'
                sh 'echo Test successful'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage completed'
            }
        }
    }
}
