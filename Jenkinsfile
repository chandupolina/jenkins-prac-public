pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('deploy') {
            when {
                not {
                    equals expected:'5', actual: "${BUILD_NUMBER}"
                } 
            }
            steps {
                echo "deployin when this condition doesnt mets"
            }
        }
    }
}
