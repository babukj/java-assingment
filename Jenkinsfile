pipeline 
{
    agent any

    stages 
	{
        stage('build') 
		{
            steps 
			{
                echo 'Build app'
            }
        }
    stage('test') 
		{
            steps 
			{
                echo 'Test app'
            }
        }
	stage('deploy') 
		{
            steps 
			{
                echo 'Deploy app'
            }
        }
	}
post 
{

        always 
		{
            emailext body: 'summary', subject: 'Pipeline status', to: 'babujillapuram@gmail.com'
        }

    }
}
