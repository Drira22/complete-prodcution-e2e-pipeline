pipeline {
    agent {
        label "Jenkins-Agent"
    }
    tools {
        jdk "Java17"
        maven "Maven3"
    }
    stages {
        stage("Cleanup Workspace") {
            steps {
                cleanWs()
            }
        }
        stage("Checkout from SCM") {
            steps {
                git url: 'https://github.com/Drira22/complete-prodcution-e2e-pipeline',
                    branch: 'main',
                    credentialsId: 'github'
            }
        }
    }
}
