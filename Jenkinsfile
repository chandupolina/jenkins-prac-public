pipeline {
    agent any 
    options {
        buildDiscarder(logRotator(numToKeepstr: '1'))
    }
    stages {
        stage ('Build') {
            steps {
                echo "hello World"
            }
        }
    }
}
