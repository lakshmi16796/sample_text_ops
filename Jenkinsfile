pipeline {
  agent any
  stages {
	  

    stage ("Edit")
    {
      steps {
        
        script {
	 		       
	env.feature = input message: 'Please enter the feature you want to build with',
                             parameters: [string(defaultValue: '',
                                          description: '',
                                          name: 'Feature')]
        echo "Entered feature is "
	echo "${env.feature}"
	input=${env.feature}
	echo "$input"
		
	array=()
	IFS='+' read -a array <<< $input
	for i in "${array[@]}"; do
  		echo "$i"
	done
      	}  
    }
  }
   }
  }

