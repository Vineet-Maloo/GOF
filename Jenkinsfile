
node()
{

  stage('git package')
	{
checkout([$class: 'GitSCM', branches: [[name: '$Branch_name']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Vineet-Maloo/GOF.git']]])
	}
  stage('package')
	{
	sh 'mvn package'
	}
  stage('archive artifacts')
	{
	archive'gameoflife-web/target/*.war'
	}

}
