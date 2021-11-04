# Team-Cyber
Cloud Innovation Center at RMIT University powered by AWS
Team Cyber



**Problem Statement:**
How might we increase the capability of ANZ SMBs to better respond to cyber-attacks by creating cyber awareness platforms ?”
 



**Solution:**
	Scenar.io - The new era of cyber security awareness training with an intuitive and a carefully curated cyber awareness cloud based platform for time-sensitive businesses. Scenar.io aims to emulate various scenarios of cyber-attacks with an intuitive and intelligent virtual platform. It has a store of different types of cyber-attack simulations that will give the users a real-time experience of an attack and its effect on their business. The training platform will feature an intelligent analytical tool which will analyse the user’s details and work out the attack scenarios customized for the specific user.




**Features:**

   - Training on recent cyber security attacks in a 3D virtual environment.
   - Scenarios are recommended as per the user's profile on the most relevant cyber security scenarios.
   - Earn a completion certificate at the end of the cyber training.
   - Suitable for all kinds of audience as the platform adopts an action-oriented training approach.
   - Can run on iOS, Android and web apps.



**Installation Steps**


- Watch the demo video and ppt (Refer Case Study @ https://www.rmit.edu.au/for-business/activator/partnerships/cloud-innovation-centre) to understand the functionality of the application.
- Cloud Formation Template (API Gateway, Lambda, DynamoDB)


  On your AWS account, create a new stack in the Cloud Formation service and upload the cloud formation template.
  
  Variables: Below are the variables needed for the app to run correctly
  
  'SENDER_EMAIL': "Email here" - Make sure this email and any email you sign up with is verified in SES
   
  'SUMERIAN_LINK':"Sumerian url here" - The public sumerian link when you deploy the sumerian scene. Make sure its the url with the ? example: https://ba1a5551859d47b6996c30d399c1fa96.ap-southeast-2.sumerian.aws/?"


- Sumerian


  The zip file SumerianBundle_TeamCyber_Final.zip contains an exported version of our sumerian scene
  To set up the completion of scenario at the end you need to change one variable in "Script 4"
  Variables:
  On line 49 of the script you need to change the url to the completeScenario endpoint from the newly deployed API
  
- AWS Amplify


  Follow the readme in the following reporsitory to deploy the app htps://github.com/scenario-cic/scenario-cic


Note:  This is just a proof of concept. If you wish to change the types of attacks, you can do so in the template under createRecommendations.
