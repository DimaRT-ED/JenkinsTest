pipeline {
   agent any
   
   stages {
	   stage('STAM') {
		   steps {
			   script {
				   sh 'echo "You are in>>> ${WORKSPACE}"'
				   sh 'echo "Your name is>>> ${USER}"'
			   }
		   }
	   }
	   stage('C') {
		   steps {
			   script {
				   if (env.LANGUAGE == 'C' || env.LANGUAGE == 'All') {
					   echo 'C file is Running'
					   echo  'Running C++ code'
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
					   echo 'Python language are Running'
					   echo  'Python code are Running'
					   sh "cat python"
				   }
			   }
		   }
	   }
   }
}
