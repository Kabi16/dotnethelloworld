pipeline {
    
    agent any
    
stages {
 stage('Checkout') {
    steps {
     git url: 'https://github.com/Kabi16/dotnethelloworld.git', branch: 'main'
     }
  }

stage('Build'){
   steps{
      bat "call Build.cmd"
    }
 }
    
stage('Publish'){
     steps{
       bat "call Publish.cmd"
     }
  }
 }
}
