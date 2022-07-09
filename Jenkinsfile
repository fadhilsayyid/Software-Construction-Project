pipeline
{
	agent any
	
	stages
	{
		stage('Build')
		{
			echo 'Build App'
		}
	}
	
	stage ('Test')
	{
		steps
		{
			echo 'Test App'
		}
	}
	
	stage ('Deploy')
	{
		steps
		{
			echo 'Deploy App'
		}
	}
	
	post
	{
		failure
		{
			emailext body: 'Summary', subject: 'Pipeline Status', to: 'fadhilsayyid01@gmail.com'
		}
	}
}

