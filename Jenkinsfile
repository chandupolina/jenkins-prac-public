pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                timeout(time: 300, unit: 'SECONDS') {
                    input(
                        message: 'Are you building the application',
                        ok: 'yes',
                        submitter: 'chandu'
                    )
                }
                echo "deploying in prod with submitter approval"
            }   
        }
    }
}
