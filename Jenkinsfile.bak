pipeline{
     
    tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
       }
      
     agent any
        stages{
            stage('clone repo'){
           
            steps{
                git credentialsId: 'mygit', url: 'https://github.com/ashisnishanka/realtimecodeNEW.git'
		    
                }
				}
             stage('Compile'){
                
                  
                steps{
                    git credentialsId: 'mygit', url: 'https://github.com/ashisnishanka/realtimecodeNEW.git'
                    sh 'mvn compile'
                }
                
            }
            stage('CodeReview'){
               steps{
                    echo "code review is succesfully"
                }
                
            }
            stage('UnitTest'){
			
                steps{
                    echo "code review is succesfully"
					sh 'mvn test'
                
                }
                
            }
            stage('MetriCheck'){
               steps{
                    echo "code review is succesfully"
                } 
                
            }
            stage('Package'){
                
               steps{
                    echo "code review is succesfully"
					sh 'mvn package'
                } 
            }
		stage(' QA deploy'){
              steps{
                    echo "code review is succesfully"
                }  
            }
			
		stage(' dev deploy'){
                
              steps{
                    echo "code review is succesfully"
                } 
            }
            
        }
    
    }
