pipeline {
    agent any
    stages {
        stage ("Install requirement") {
            steps {
                echo "Installing requirement from pip install"
                echo "Workspace: ${workspace}"
                bat "python -m virtualenv venv && venv\\Scripts\\activate && pip install -r requirement.txt && venv\\Scripts\\deactivate.bat"
            }
        }
        stage ("Run tests") {
            script {            
                TEST_FILE = "${workspace}\\test_siq_tests.py"
            }
            steps {
                browserstack(credentialsId: '373e6a65-62a7-4548-ba57-3243d5441127', localConfig: [localOptions: '', localPath: ""]) {                
                    echo "venv\\Scripts\\activate && python -m pytest \"${TEST_FILE}\" && venv\\Scripts\\deactivate.bat"
                }
            }
        }
    }
}
