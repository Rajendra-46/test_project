pipeline {  
 agent any  

 stages {  
  stage('Checkout') {  
   steps {
    git credentialsId: 'admin', url: 'https://github.com/Rajendra-46/test_project.git', branch: 'main'   }  
  }  
 stage('Build') {  
   steps {  
    bat 'dotnet build C:\\Users\\prasad\\Documents\\repos\\c#project\\test_project\\c#project.sln --configuration Release' 
   }  
  }  
  stage('Test') {  
   steps {  
    bat 'dotnet test C:\\Users\\prasad\\Documents\\repos\\c#project\\test_project\\c#project.csproj --logger:trx'  
   }  
  }
 }
}
