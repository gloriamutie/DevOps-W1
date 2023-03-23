pipeline{
    agent any
    tools{
        nodejs "node"
    }
    
    stages{
        stage('Start'){
            steps{
                echo 'build has started'
            }
        }
        stage('clone repository from github'){
            steps{
                git url: 'https://github.com/gloriamutie/DevOps-W1.git', branch: 'master'
            }
        }
          stage('install dependencies'){
            steps{
               sh '''
               npm install
               '''            

            }
        }
        stage('run tests'){
            steps{
               sh 'npm test'
            }
        }
        stage('end  build'){
            steps{
                sh '''
                echo "end build"
                '''
            }
        }
    }

}