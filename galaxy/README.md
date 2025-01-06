## Ansible Galaxy

- Ansible Galaxy is a marketplace for ansible roles, from where we can install/ use the existing ansible roles made by great devs out there.
- Role in ansible is the way to make your ansible playbook modular, scalable, readable and reusable. This comes in handy when your playbook is going to contain more than 1000s of line.

### Command

`ansible-galaxy role init role-name`

- A above command will generate a dir with `role-name` and it will contain a list dir as defaults, files, handlers, meta, tasks, templates, tests, & vars.
- Each of these dir serve their own purposes such as inside `tasks` dir , we can have a `main.yaml` and list our config tasks, etc.
- When using `ansible-roles` we need to specify `roles` attribute in our `playbook.yaml` file (in my case it is `my-first-playbook.yaml`)

<br />
<br />

`ansible-galaxy role install name-of-role-from-market-place`

- Here I am installing a already present role from [galaxy.ansible.com](galaxy.ansible.com) i.e. **bsmeding docker** which does nothing but installing and configuring **Docker** on your host machines.