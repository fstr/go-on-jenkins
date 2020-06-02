pipeline {
    agent any
    tools {
        go 'go-1.14.4'
    }
    environment {
        GO111MODULE = 'on'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Compiling...'
                sh 'go version'
                sh 'go build main.go'
                sh './main'
            }
        }
    }
}
