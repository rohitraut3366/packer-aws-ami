pipeline{
    stages{
        stage("packer"){
            // agent{
            // label "packer"
            // }
            steps{
                echo "Build Started"
                git url: "https://github.com/rohitraut3366/packer-aws-ami.git" branch: "master"
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