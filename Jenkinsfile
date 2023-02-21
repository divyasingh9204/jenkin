pipeline {
    agent any
    
    stages {
        
        stage("build") {
            steps {
                echo 'this is build stage'
            }
        }
        stage("test") {
            
            steps {
                echo 'this is test stage'
                snDevOpsChange(changeRequestDetails: """{"setCloseCode": false,"pollingInterval":"10","abortOnChangeCreationFailure": true}""")
            }
        }
        stage("deploy") {
            steps {
                echo 'this is deploy stage'
            }
        }
        
    }   
}
