
pipeline {
 agent any
 environment {
  dotnet = 'C:/Program Files/dotnet/dotnet.exe'
 }
 stages {
  stage('Restore PACKAGES') {
   steps {
    bat "dotnet restore --configfile NuGet.Config"
   }
  }
  stage('Clean') {
   steps {
    bat 'dotnet clean'
   }
  }
  stage('Build') {
   steps {
    bat 'dotnet build --configuration Release'
   }
  }
 }
}
