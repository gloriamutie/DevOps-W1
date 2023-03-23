pipeline { 
  agent any
   tools{
        nodejs "node"
    }
  stages { 
    stage('clone repository') {

      steps { 
        git 'https://github.com/gloriamutie/DevOps-W1.git',branch: 'master'
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
