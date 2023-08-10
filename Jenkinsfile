//Start pipeline
pipeline{
  //Agent declaration
  agent{
    label 'jenkins_agent'
  }
  //Tools declaration
  tools{
    maven 'mymaven'
  }
  //Stages declaration
  stages{
    //Code checkout
    stage('Code checkout from VCS'){
      steps{
        git 'https://github.com/prakrishna2004/DevOpsClassCodes.git'
      }
    }
    //Code compilation
    stage('Code compilation'){
      steps{
        mvn 'compile'
      }
    }
   //Code compilation
    stage('Code Compilation'){
      steps{
        mvn 'compile'
      }
    }
    //Code review
    stage('Code Review'){
      steps{
        mvn 'pmd:pmd'
      }
    }
    //Code testing
    stage('Code Testing'){
      steps{
        mvn 'test'
      }
    }
    //Code packaging
    stage('Code package'){
      steps{
        mvn 'package'
      }
    }
  }//End stages
}//End pipeline
