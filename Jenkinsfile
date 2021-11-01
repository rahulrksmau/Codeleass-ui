pipeline {
    agent any
    stages {
        stage ("Run tests") {
            steps {
                browserstack(credentialsId: '373e6a65-62a7-4548-ba57-3243d5441127', localConfig: [localOptions: '', localPath: ""]) {                
                    tpJobRun agentId: 'upP2B4Jki0e3aK5QD0wZzQ', executionParameters: '', jobId: 'lgJdDeJlDUGUiytSP-f0AA', junitResultsFile: '', projectId: 'MTLk7RYTv0SP7IaT0Sof0Q', waitJobFinishSeconds: 30
                }
            }
        }
    }
}
