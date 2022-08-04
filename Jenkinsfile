pipeline {
   agent any
   
   stages {
	   stage('Entry'){
		   steps {
			   sh '''
			   echo U chouse to run a env.LANGUAGE 
			   '''
		   }
	   }
	   stage('C') {
		   steps {
			   script {
				   if (env.LANGUAGE == 'C' || env.LANGUAGE == 'All') {
					   echo 'C file is Running'
					   sh 'cat c'
				   }
			   }
		   }
	   }
	   stage('Bash') {
		   steps {
			   script {
				   if (env.LANGUAGE == 'BASH' || env.LANGUAGE == 'All') {
					   echo 'Bash file is Running'
					   sh 'cat bash'
				   }
			   }
		   }
	   }
	   stage('Python') {
		   steps {
			   script {
				   if (env.LANGUAGE == 'PYTHON' || env.LANGUAGE == 'All') {
					   echo  'Python file is Running'
					   sh 'cat python'
				   }
			   }
		   }
	   }
   }
}
