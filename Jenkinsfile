pipeline {  
 agent any  
 environment {  
  dotnet = 'C:\\Program Files\\dotnet\\dotnet.exe'  
 }  
 stages {  
  stage('Checkout') {  
   steps {
       git credentialsId: 'admin', url: 'https://github.com/Rajendra-46/test_project.git', branch: 'main'
   }  
  }  
 stage('Build') {  
   steps {  
    bat 'dotnet build C:\\Users\\prasad\\Documents\\repos\\c#project\\c#project.sln --configuration Release' 
    //bat 'dotnet build C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\HRMPipelines\\jenkins-demo\\HRM\\HRM.sln --configuration Release'  
   }  
  }  
  stage('Test') {  
   steps {  
    bat 'dotnet test C:\\Users\\prasad\\Documents\\repos\\c#project\\test_project\\c#project.csproj --logger:trx'  
   }  
  }
  
  


 }  
}
