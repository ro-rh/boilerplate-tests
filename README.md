ential# README for: Project A

## About

> [!NOTE]
> Runs on RHEL9 Only

> [!TIP]
> Refresh between pulls

> [!IMPORTANT]
> Ensure no security data is hardcoded

> [!WARNING]
> Don't push to master without approval

> [!CAUTION]
> May crash if variables aren't correct



This code is used for doing very complicated things, such as solving a Rubik's cube. It is important to have the following background information about why the code is needed for the project. Project 2 is scheduled to play Tetris on Mondays, if the Rubik's cube isn't completed, the Tetris will fail. 


| Info | About |
| ------ | ------ |
| Version | v1.1|
| GitHub | [criticalserver/topsecret/supersecret]  |
| Documentation | [documentation/supersecret.pdf] |
| Environment | Dev |
| Code Owner | John Smith - john.smith@example.com |

## Features
- Boilerplate file to help give structure
- Ran in the test environment
- Whatever quick easy to read info you think would help to understand what it does/how it works etc


## Vars

Anything info about vars entered here

| Setting | Parameters | Additional Info |
| ------ | ------ | ------ |
| File List | sequential-files | List of Files to Remove |


## Inputs & Output

Under condition A the expected output is B. If input B = 1 output B defaults to 2

## Example Code

```yaml
# roles/example/tasks/main.yml
- name: Install the correct web server for RHEL
  import_tasks: redhat.yml
  when: ansible_facts['os_family']|lower == 'redhat'

- name: Install the correct web server for Debian
  import_tasks: debian.yml
  when: ansible_facts['os_family']|lower == 'debian'

# roles/example/tasks/redhat.yml
- name: Install web server
  ansible.builtin.yum:
    name: "httpd"
    state: present

# roles/example/tasks/debian.yml
- name: Install web server
  ansible.builtin.apt:
    name: "apache2"
    state: present
```

## Support

To get support
1. Contact Team A
1. Contact Product Owner

Process Flow for Further Support

```mermaid
flowchart LR
    A[Go to Service Now] --> B[Raise Ticket Under 'Project A']
    B --> C{Issue Resolved?}
    C -->|Yes| D[Good]
    C -->|No| E[Contact PM]
```
    
## Team

| Name | Role |  Team | Orginisation | E-Mail |
| ------ | ------ | ------ | ------ | ------ |
| John Smith | Engineer | Project A Team | Company A | John.Smith@example.com |
| Sherlock Smith | Tester | Project B Team | Red Hat | Sherlock.Smith@example.com |


[//]: # (Add any referenced links here)

   
   [RedHat]: <http://redhat.com>
   [file]: <https://github.com/test/projects/testproject1/README.md>

