pipeline
{
	agent any
	
	stages
	{
		stage ('Build Docker Image')
		{
			steps
			{
				script
				{
					dockerapp = docker.build("aluizsys/kube-news:v${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
				}
			}
		}
	}
}