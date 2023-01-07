# Local Ansible playground

This project is just for educational purposes.

In this example, my only server at the moment is my old Lenovo x270, tied next to the router xD

Server distro: Fedora Server 37

## **Installation**

### ***Software***

First, make sure that u have an ansible installed.

**Debian/Ubuntu**:

```(bash)
sudo apt install ansible yamllint ansible-lint
```

**Fedora/CentOS**:

```(bash)
sudo dnf install ansible yamllint ansible-lint
```

**Thru pip** (make sure that PATH to ansible is set)**:**

```(bash)
pip install ansible
```

### ***Roles (Custom ansible modules)***

This project uses some custom roles, which u can install to this project, using `ansible-galaxy`:

```(bash)
ansible-galaxy install -p ./roles -r requirements_ansible.yml
```

### ***SSH keys***

Don`t forget to generate key to access to ansible user on hosts:

```(bash)
ssh-keygen -t rsa -b 4096 -C "<your_email@example.com>" -f $HOME/.ssh/id_rsa_ansible
```
