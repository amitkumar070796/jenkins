pipeline{
    agent any
    stages{
        stage("check date and time"){
            steps{
                sh 'date'
            }
        }
        stage("present working directory"){
            steps{
                sh 'pwd'
            }
        }
        stage("check calender"){
            steps{
                sh 'cal'
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
