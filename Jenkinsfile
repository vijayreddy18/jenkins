@Library('shared-library') _
pipeline {
    agent any
    environment {
        JIRA_URL = 'https://chilukashirish.atlassian.net'
        JIRA_CREDENTIALS = credentials('personal-token')
    }

    stages {
     stage('Move Jira Ticket') {
       steps {
moveJiraTicket(issueKey: 'TCS-1', destinationProject: 'TCS', destinationIssueStatus: 'InProgress')
}
}
    }
}
