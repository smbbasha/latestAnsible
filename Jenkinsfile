node {   
  stage('Git-Checkout') {
   git 'https://github.com/Sandeepkr93/AnsibleInfraNew.git'
  }
  
  def project_ansible="ansible-01/"
dir(project_ansible) {
   stage('ansible-deploy') {
   sh 'ansible-playbook  --key=/var/lib/jenkins/devop-aws-demo.pem  web-playbook.yaml -u ubuntu -v'
  }
  }
}
