
node {
   stage('SCM Checkout'){
       git 'https://github.com/javednaikawadi/picassotechnology'
    }
   stage('Compile-Package'){
	 //get mvn home path
	def mvnHome =  tool name: 'maven-3', type: 'maven'
	 sh "${mvnHome}/bin/mvn package"
    }
   stage('Email Notification'){
	mail bcc: '', body: '''Hi,
	Welcome!!

	Regards,
	Javed.''', cc: '', from: '', replyTo: '', subject: 'Jenkins Picasso Email', to: 'javednaikawadi@gmail.com'	
   }
}

