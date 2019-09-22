
node()
{
  stage('git package')
	{
	git 'https://github.com/Vineet-Maloo/GOF.git'
	}
  stage('package')
	{
	sh 'mvn package'
	}
  stage('archive artifacts')
	{
	archiveArtifacts '/gameoflife-web/target/*.war'
	}

}
