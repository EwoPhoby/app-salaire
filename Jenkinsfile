node{
    stage('vérif') {
      checkout scm
    }
    stage('clone'){
      git 'https://github.com/EwoPhoby/app-salaire'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,          
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
