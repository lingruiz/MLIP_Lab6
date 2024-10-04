pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''#!/bin/bash
                echo 'In C or Java, we can compile our program in this step'
                echo 'In Python, we can build our package here or skip this step'
                '''
            }
        }
        stage('Test') {
            steps {
                sh '''#!/bin/bash
                echo 'Test Step: We run testing tool like pytest here'


                # Create a virtual environment
                # python3 -m venv lab6

                # Activate the virtual environment
                # source mlip/bin/activate

                # Upgrade pip within the venv
                # pip install --upgrade pip


                # Install pytest
                # pip install pytest pandas numpy scikit-learn

                # run pytest
                pytest

                # deactivate the virtual environment
                deactivate
                '''

            }
        }
        stage('Deploy') {
            steps {
                echo 'In this step, we deploy our porject'
                echo 'Depending on the context, we may publish the project artifact or upload pickle files'
            }
        }
    }
}
