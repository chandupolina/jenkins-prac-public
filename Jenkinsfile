pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'Production'
    }
    stages {
        stage ('Deploy') {
            when {
                equals expected: 'Production', actual: "${DEPLOY_TO}"
            }
            steps {
                echo "Deploying to Production"
            }
        }
    }
}
