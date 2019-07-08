pipeline{
    agent any
    stages{
        stage('clone'){
            steps{
                bat "rm -rf maven"
                bat "git clone https://github.com/MOHD-WAQAR/maven.git"
                bat "mvn clean"
            }
        }
        stage('test'){
            steps{
                bat "mvn test"
            }
        }
        stage('deploy'){
            steps{
                bat "mvn package"
            }
        }
    }
}
