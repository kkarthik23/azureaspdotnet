# azureaspdotnet
Sample project with Azure devops pipeline which integrates with Sonar Cloud
In your project settings goto pipeline, goto service connections create the service connection for sonar cloud
provide the sonar cloud token 

### Replace relevant sections for Synk integration
---

- task: SnykSecurityScan@0
  inputs:
    serviceConnectionEndpoint: 'snykToken'
    testType: 'app'
    monitorWhen: 'always'
    failOnIssues: true

---
