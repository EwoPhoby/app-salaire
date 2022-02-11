node{
    stage('vérif') {
      checkout scm
    }
    stage('clone'){
      git 'https://github.com/EwoPhoby/app-salaire.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,          
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
