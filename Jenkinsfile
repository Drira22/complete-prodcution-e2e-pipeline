pipeline{
    agent{
        label "Jenkins-Agent"
    }
    tools{
        jdk "Java17"
        maven "Maven3"
    }
    stages{
        stage("Cleanup Workspace"){
            steps{
                cleanWs()
            }
        }
    }
}