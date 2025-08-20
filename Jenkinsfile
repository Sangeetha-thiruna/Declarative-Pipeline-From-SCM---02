pipeline {
    agent any
    stages{
        stage ('Checkout'){
            steps{
                echo 'Checkout Source Code'
                git branch: 'main',url:'https://github.com/Sangeetha-thiruna/Declarative-Pipeline-From-SCM---02.git'
            }
        }
        stage ('Build'){
            steps{
                echo 'Building the pipeline'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing the pipeline'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying the pipeline'
            }
        }
    }
    post{
        success{
            echo 'Pipeline done Successfully'
        }
        failure{
            echo 'Pipeline Fails'
        }
        always{
            echo 'This will runs pipeline success or failure'
        }
    }
}