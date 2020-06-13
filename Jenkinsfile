
node {
	def mvn = tool (name: 'maven3', type: 'maven') + '/bin/mvn'
   stage('SCM Checkout'){
       url: 'https://github.com/javednaikawadi/picassotechnology'
    }
   stage('Compile-Package'){
	 //get mvn home path
	//def mvnHome =  tool name: 'maven-3', type: 'maven'
	   sh "${mvn} clean -X package"
    }
}

