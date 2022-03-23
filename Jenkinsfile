pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh """
               echo "Building Artifact"
               """
           }
       }
       stage('Reading branch wise info')
       {
       when
       {
       branch "feature*"
       }
       steps
       {
       echo " It is only for Feature Branch"
       }
       }
      stage('Deploy Code') {
          steps {
               sh """
               echo "Deploying Code"
               """
          }
      }
   }
}
