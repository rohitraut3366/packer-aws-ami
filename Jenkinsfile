pipeline{
    agent { 
        label "packer"
    }
    stages{
        stage("packer-build"){
            steps{
                echo "Build Started"
                git branch: 'master', url: 'https://github.com/rohitraut3366/packer-aws-ami.git'
                sh "packer build ."
                echo "Build Ended"
            }
            post{
                success{
                    echo "executed successfully"
                }
                failure{
                    echo "execution failed"
                }
            }
        }
    }
}