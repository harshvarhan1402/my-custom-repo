pipeline {
    agent any
    stages {
        stage('list home directory contents') {
            when {
                anyOf {
                    expression { params.all == true }
                    expression { params.first == true }
                }
            }
            steps {
                sh 'cd /home/ubuntu/; ls'
            }
        }
        stage('hello') {
            when {
                anyOf {
                    expression { params.all == true }
                    expression { params.second == true }
                }
            }
            steps {
                echo 'hello'
            }
        }
        stage('hardik') {
            when {
                anyOf {
                    expression { params.all == true }
                    expression { params.third == true }
                }
            }
            steps {
                sh 'cd /home/ubuntu/; cat hardik'
            }
        }
    }
}
