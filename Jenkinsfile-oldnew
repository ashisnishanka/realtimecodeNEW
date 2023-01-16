pipeline
{
 agent any
 
 stages{
 
 stage("git checkout")
 {
   steps
   {
     
     git credentialsId: 'mygitnew1', url: 'https://github.com/ashisnishanka/realtimecodeNEW.git'
     echo "git checkout"
   }
}
 stage("compile")
 {
   steps
   {
       sh 'mvn compile'
       echo "compile job"
   }
}
stage("test")
 {
   steps
   {
     sh 'mvn test'
     echo "test job"
   }
}
stage("package")
 {
   steps
   { 
       sh 'mvn package'
     echo "package job"
   }
}

  }
 }
