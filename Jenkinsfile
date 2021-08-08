pipeline{
    stages{
        stage("packer"){
            agent{
            label "packer"
            }
            steps{
                echo "Build Started"
                git url: ""
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
