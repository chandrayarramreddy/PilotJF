node{
   
   ws("workspace/${env.JOB_NAME}/${env.BRANCH_NAME}".replace('%2F', '_')) {
   def mvnHome
   // for display purposes
      // Get some code from a GitHub repository
      https://github.com/chandrayarramreddy/PilotProject.git
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           
      mvnHome = tool 'M2_HOME'
  
   stage('Build') {
      // Run the maven build
   //   if (isUnix()) {
    //     sh "'${mvnHome}/bin/mvn' clean package"
     // } else {
         bat(/"${mvnHome}\bin\mvn" clean package/)
      //}
   }
   
   }
}
