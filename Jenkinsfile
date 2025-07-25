pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'Production'
    }
    stages {
        stage ('Deploy') {
            When {
                equals expected: 'Production', actual: '${DEPLOY_TO}'
            steps {
                echo " Deploying to Production"
            }
            }
            
        }
    }
}
