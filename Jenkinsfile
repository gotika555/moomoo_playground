pipeline {
    //agent is required
    agent any
    //add stages for pipeline
    stages{
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
            }
            stage('Docker build'){
                steps{
                    sh(script:"""
                    docker-compose build
                    """
                    )


                }
            }
    }
}