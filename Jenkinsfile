pipeline{
    agent{
        label "agent-jenkins1"
    }
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }

        }
    }
        stages{
        stage("Check out from SCM"){
            steps {
                git branch: 'main', credentialsId: 'git-hub', url: 'https://github.com/ibanoba/complete-prodn-e2e-pipeline'
            }

        }
    }
}