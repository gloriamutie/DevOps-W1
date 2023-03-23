pipeline { 
  agent any
   tools{
        nodejs "node"
    }
  stages { 
    stage('clone repository') {

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

        
  }
}
