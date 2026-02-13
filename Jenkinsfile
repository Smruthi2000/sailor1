pipeline{
    agent {
        lable 'slave1'
    }
    tools{
        maven 'maven'
    }
    stages{
        stage('checkout '){
            steps{
            git branch: 'main', url: 'https://github.com/Smruthi2000/sailor1.git'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean verify'
            }
        }
    }
}