pipeline {
  agent any
  options { timestamps() }
  stages {
    stage('Build') {
      steps { echo 'Build — Tool: npm (or Maven/Gradle)' }
    }
    stage('Unit & Integration Tests') {
      steps { echo 'Tests — Tool: Jest (or JUnit/Mocha)' }
    }
    stage('Code Analysis') {
      steps { echo 'Static analysis — Tool: ESLint (or SonarQube)' }
    }
    stage('Security Scan') {
      steps { echo 'Dependency scan — Tool: OWASP Dependency-Check' }
    }
    stage('Deploy to Staging') {
      steps { echo 'Deploy — Tool: Ansible (or Docker Compose)' }
    }
    stage('Integration Tests on Staging') {
      steps { echo 'E2E/API — Tool: Newman (Postman CLI)' }
    }
    stage('Deploy to Production') {
      steps { echo 'Promote — Tool: Ansible (or Terraform/kubectl)' }
    }
  }
}
JENKINS