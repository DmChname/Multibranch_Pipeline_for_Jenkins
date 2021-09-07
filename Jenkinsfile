pipeline
{
    agent {label "Linux"}
    stages
    {
        stage('Stage Hello')
        {
            steps
            {
                echo 'Hello world!'
            }
        }
        stage('cat README')
        {
	    when
	    {
		branch "fix-*"
	    }
            steps
            {
		sh '''
                  cat README.md
		'''
            }
        }
    }
}
