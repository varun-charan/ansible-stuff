Learnings:
	1. Ansible's default inventory file is: /etc/ansible/hosts
	2. You can create a custom one and override the hosts file in every ansible command with the "-i" option.
	3. If the servers return "Failed to connect" error, run a ping on them using "ansible -m ping all" and then re-run the playbook. It'll work if the ping works.
	4. For common variables to a group, add to group_vars/ folder in the file named same as the target group.
	5. For host-level variables, either add them against the hosts in the inventory file or use host_vars/ folder.
