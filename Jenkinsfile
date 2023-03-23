pipeline { 
  agent any
  stages { 
    stage('clone repository') {
      steps { 
        git 'https://github.com/gloriamutie/DevOps-W1.git'
      }
    }
    stage('Install Dependencies') {
            steps {
                sh 'npm install'
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
