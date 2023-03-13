# Stephane ROBERT ansible Snippets for Visual Studio Code

This Visual Studio Code extension has snippets to help you write your Ansible
code when you are recommendations on my [personal blog](https://blog.stephane-robert.info/)

![ansible snippets vscode](https://github.com/stephrobert/ansible-snippets/raw/main/img/sr-ansible-snippet.gif)

## List of snippets

**Format :**

* module
  * text to invoque

* playbook
* block
* ansible.builtin.add_host:
  * "add host to group"
* ansible.builtin.debug:
  * "debug a task"
* ansible.builtin.package:
  * "install a package"
* ansible.builtin.package:
  * "copy a file"
* ansible.builtin.template:
  * "generate a file from a template"
* ansible.builtin.file:
  * "create a file"
  * "touch a file"
  * "create a directory"
* ansible.builtin.service:
  * "start a service"
  * "stop a service"
  * "enable a service"
  * "disable a service"
* ansible.builtin.set_fact:
  * "compute a variable"
  * "set a variable"
* ansible.builtin.lineinfile:
  * "include a line in a file"
* ansible.builtin.stat:
  * "status of a file or a directory"
* ansible.builtin.unarchive:
  * "unarchive a compressed file"
* ansible.builtin.import_tasks:
  * "Import tasks"
* ansible.builtin.include_tasks:
  * "Include tasks"
* ansible.builtin.import_playbook:
  * "Import playbook"
* ansible.builtin.import_role:
  * "Import role"
* ansible.builtin.include_role:
  * "Include a Role"
* ansible.builtin.assert:
  * "Assert"

<!-- set_fact, stat, blockinfile, lineinfile, assert, includes, wait_for, import_tasks, unarchive
- name: Add os specific variables
  ansible.builtin.include_vars: "{{ loop_vars }}"
  with_first_found:
    - files:
        - "{{ ansible_distribution | lower }}-{{ ansible_distribution_version }}.yml"
        - "{{ ansible_distribution | lower }}-{{ ansible_distribution_major_version }}.yml"
        - "{{ ansible_distribution | lower }}.yml"
        - "{{ ansible_os_family | lower }}.yml"
        - "{{ ansible_system | lower }}.yml"
        - "main.yml"
      paths:
        - "vars"
  loop_control:
    loop_var: loop_vars -->