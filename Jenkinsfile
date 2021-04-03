node('master') 
{
    stage('ContinuousDownload')
    {
       git 'https://github.com/rajesh444/jenkin_DP.git'
    }
    stage('ContinuousBuild')
    {
       sh 'mvn package'
    }
    stage('ContinuousDeployment')
    {
     sh 'scp /home/ubuntu/.jenkins/workspace/DerPipeline/webapp/target/webapp.war ubuntu@172.31.26.148:/var/lib/tomcat9/webapps/qaapp.war'  
	            
		 
    }
    }
