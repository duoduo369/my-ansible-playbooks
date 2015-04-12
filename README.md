my-ansible-playbooks
===

Usage
---

    sudo apt-get install ansible
    sudo apt-get install sshpass
    mkdir ~/projects
    sudo ln -s ~/projects /opt
    git clone https://github.com/duoduo369/my-ansible-playbooks.git /opt/projects
    sudo mkdir -p /etc/ansible
    sudo cp /opt/projects/my-ansible-playbooks/ansible.cfg /etc/ansible/ansible.cfg
    cp /opt/projects/my-ansible-playbooks/ansible_hosts ~/

初始化linux脚本 init_linux_playbook.yaml
---

playbook主要工作:

1. 安装我自己的各种linux配置
2. 个人经验项目skill_issue
3. 安装定制的oh-my-zsh
4. 安装定制的vim(janus)

    cd /opt/projects/my-ansible-playbooks
    ansible-playbook init_linux_playbook.yaml --ask-pass
