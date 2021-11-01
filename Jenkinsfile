pipeline {
    agent any
    stages {
        stage ("Run tests") {
            steps {
                browserstack(credentialsId: '373e6a65-62a7-4548-ba57-3243d5441127', localConfig: [localOptions: '', localPath: ""]) {                
                    tpJobRun agentId: 'vHHgIHKLRkq8wheiuOFY9w', executionParameters: '', jobId: 'E6wU5BGAQ0mpZa6kXtyOyw', junitResultsFile: '', projectId: 'MTLk7RYTv0SP7IaT0Sof0Q'
                }
            }
        }
    }
}
