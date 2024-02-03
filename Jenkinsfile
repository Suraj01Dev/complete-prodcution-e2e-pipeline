pipeline{

    agent{
        label "jenkins-ssh-agent"
    }

    tools{
        jdk "java17"
        maven "Maven3"

    }

    stages{
        stage("Clean Workspace"){
            steps{
                cleanWs()
            }

        }

        stage("Git Checkout SCM"){

            steps{
                git branch:"master", credentialsId: 'github', url: 'https://github.com/Suraj01Dev/complete-prodcution-e2e-pipeline'
            }
        }

    }


}