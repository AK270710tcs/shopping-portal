pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the build job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'npm tets'
      }
    }

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
    }

<<<<<<< HEAD
    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'                
            }
        }
=======
    stage('Archive') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
>>>>>>> 6bdb4d67272dbdc60540c0e595f3d6e0cf0997c3
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }
<<<<<<< HEAD
    
}

=======

  }
}
>>>>>>> 6bdb4d67272dbdc60540c0e595f3d6e0cf0997c3
