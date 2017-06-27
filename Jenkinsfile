pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            if (env.BRANCH_NAME == 'master') {
                echo 'I only execute on the master branch'
            } 
            else {
                echo 'I execute elsewhere'
                }
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}