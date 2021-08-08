pipeline{
    agent packer
    stages{
        stage("packer"){
            steps{
                echo "Build Started"
                git branch: 'master', url: 'https://github.com/rohitraut3366/packer-aws-ami.git'
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