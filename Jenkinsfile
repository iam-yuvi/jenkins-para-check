pipeline {
    agent any

    parameters {
        choice(
            name: 'branchName',
            choices: ['develop', 'main', 'staging', 'testing'],
            description: 'Select branch name'
        )
    }

    stages {
        stage('Build') {
            steps {
                echo "Selected branch: ${params.branchName}"
            }
        }
    }
}
