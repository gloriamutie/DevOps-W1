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
  }
}