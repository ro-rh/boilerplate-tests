# postbuild Ansible Role

## About
> Note: This role currently ONLY supports RHEL9


| Info | About |
| ------ | ------ |
| Version | v1.1|
| GitHub | [criticalserver/topsecret/supersecret]  |
| Documentation | [documentation/supersecret.pdf] |
| Code Owner | John Smith - john.smith@example.com |

## Features
- Boilerplate file to help give structure
- Ran in the test environment
- Whatever quick easy to read the info you think would help to understand what it does/how it works etc


## Vars

Anything info about vars entered here

| Setting | Parameters | Additional Info |
| ------ | ------ | ------ |
| File List | postbuild_files | List of Files to Remove |




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

To raise a support ticket:
    1. Go to wherever
    2. Click whatever
    3. Wait
    4. Done!
    
## Team

| Name | Role |  Team | Orginisation | E-Mail |
| ------ | ------ | ------ | ------ | ------ |
| John Smith | Engineer | Project A Team | Company A | John.Smith@example.com |
| Sherlock Smith | Tester | Project B Team | Red Hat | Sherlock.Smith@example.com |


[//]: # (Add any referenced links here)

   
   [RedHat]: <http://redhat.com>
   [file]: <https://github.com/test/projects/testproject1/README.md>

