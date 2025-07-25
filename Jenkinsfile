pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('paralllel_stages') {
            parallel {
                stage ('buid') {
                    steps {
                        echo "building stage "
                        sh "sleep 15"
                    }
                }
                stage ('sonar scan') {
                    steps {
                        echo "code analysis"
                        sh "sleep 15"
                    }
                }
                stage ('deploy') {
                    steps {
                        echo "deploying to prod"
                        sh "sleep 15"
                    }
                }
            }
        }
        stage (' second stage ') {
            steps {
                echo " second stage "
            }
        }
    }
}
