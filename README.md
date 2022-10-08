# ansible-windows-exporter
Ansible role to install Prometheus Node Exporter on windows server

## Installation

Create requirements.yml file

```
# Include windows-exporter role
- src: https://github.com/FastMT/ansible-windows-exporter.git
  name: windows-exporter
  version: "v1.0.1"
```

Install external module into ~/.ansible/roles folder

```
ansible-galaxy install -r requirements.yml
```

## Usage

playbook.yml:

```
# Install windows node exporter
- role: "windows-exporter"
```        

see [defaults](defaults/main.yml) for optional variables
