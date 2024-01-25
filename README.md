# postbuild Ansible Role

## About
> Note: This role currently ONLY supports RHEL9


| Info | About |
| ------ | ------ |
| Version | v1.1|
| GitHub | [criticalserver/topsecret/supersecret][PlGh] |
| Documentation | [documentation/supersecret.pdf][PlGd] |
| Code Owner | John Smith - john.smith@example.com |

## Features
- Boilerplate file to help give structure
- Ran in test environment
- Whatever quick easy to read info you think would help to understnad what it does/howit works etc


## Vars

Anything info about vars entered here

| Setting | Parameters | Additional Info |
| ------ | ------ | ------ |
| File List | postbuild_files | List of Files to Remove |
| GitHub | [criticalserver/topsecret/supersecret][PlGh] |
| Documentation | [documentation/supersecret.pdf][PlGd] |
| Code Owner | John Smith - john.smith@example.com |



## Inputs & Output

Under the condition A the expected output is B. If input B = 1 output B defaults to 2

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


[//]: # (Add any refferenced links here)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
