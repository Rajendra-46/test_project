pipeline {  
 agent any  
 environment {  
  dotnet = 'C:\\Program Files\\dotnet\\dotnet.exe'  
 }  
 stages {  
  stage('Checkout') {  
   steps {
       bat "git clone --single-branch --branch main https://github.com/Rajendra-46/test_project.git"
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
  
  




