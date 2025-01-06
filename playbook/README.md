## Playbook 

- Playbook in ansible consists of `plays` also can be referred as tasks where each playbook can have multiple.
- Each `play` has something to do with configuring a certain service/ server/ application (can be a simple index.html) onto the hosts.
- Hosts in ansible are nothing but the Public IPs of VMs (in my case, I am using AWS EC2 Ubuntu instances of type t2.micro )
- Hosts can also be grouped and playbook can run the tasks for a certain group. Eg: `hosts: db` meaning the tasks would run only for instances grouped as `db`

### Command

`ansible-playbook -i inventory-file-path playbook-name.yaml`

- Inventory or `inventory.ini` is the file containing the lists of host IPs (can be grouped or default all)

- With respect to the current dir structure, the command becomes:\
`ansible-playbook -i ../inventory.ini my-first-playbook.yaml`