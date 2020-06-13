
node {
	def mvn = tool name: 'maven-3', type: 'maven'
   stage('SCM Checkout'){
       url: 'https://github.com/javednaikawadi/picassotechnology'
    }
   stage('Compile-Package'){
	 //get mvn home path
	//def mvnHome =  tool name: 'maven-3', type: 'maven'
	   sh "${mvn}/bin/mvn clean -X package"
    }
}

