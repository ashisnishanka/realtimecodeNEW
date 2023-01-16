pipeline
{
   tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
 agent any
 stages
 {
   stage("git checkout")
   {
     steps
	 { 
	   echo "my git hub code "	
	   git credentialsId: 'mygitpassword', url: 'https://github.com/ashisnishanka/realtimecodeNEW.git'
	 }   
   }
   
   stage("compile")
   {
     steps
	 { 
	   echo " compile "
	   sh 'mvn compile'
	 } 
   }
   
   stage("test")
   {
     steps
	 { 
	   echo " test "
	   sh 'mvn test'
	  }
    }
   
   stage("package")
   {
     steps
	 { 
	   echo " package "
	   sh 'mvn package'
	 }
   }
 }

}
