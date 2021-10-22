pipeline {
  agent {
    node {
      label 'Asset.Slabe2'
    }

  }
  stages {
    stage('a1') {
      steps {
        sh '''if [ ! -e ./Assets ]; then
	echo "start clone sekai_client"
    git clone git@github.com:ColorfulPalette/sekai_client.git .
	git checkout -B ${client_branch} origin/develop1.11.0
    echo "finish cloned sekai_client"
fi'''
      }
    }

  }
}