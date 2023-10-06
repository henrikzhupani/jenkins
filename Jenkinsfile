pipeline {
    agent any
    stages {
        stage('Build for Test Branch') {
            when {
                expression {
                    return env.BRANCH_NAME == 'test'
                }
            }
            steps {
                // Your build steps for the 'test' branch here
                sh 'echo "Building the branch: $BRANCH_NAME"'
            }
        }
    }
}
