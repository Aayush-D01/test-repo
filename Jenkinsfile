pipeline {
    agent {
        node {
            label "docker-agent-1"
        }
    }
    triggers{
        pollSCM('19 10 * * 5')
    }
    stages {
        stage('Build') {
            steps {
                echo "First stage: build"
            }
        }
        stage('Test') {
            steps {
                echo "Second stage: test"
            }
        }
        stage('Deploy') {
            steps {
                echo " Third stage: deploy"
            }
        }
    }
}
