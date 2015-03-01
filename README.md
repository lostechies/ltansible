lostechies ansible scripts

Make sure you have hosts populated in `production` file

Example:
    
    [webservers]
    11.11.11.11

    [dbservers]
    22.22.22.22

How to run:

    ansible-playbook web.yaml -i production -u [username] -k

The `-k` will prompt you for the password.  Look at ansible docs for how to avoid doing this.

**Make sure to populate the variables in:**

    roles/common/vars/main.yaml
    web.yaml
    db.yaml

Suggestions and best practices welcome.

Ansible Documentation can be found [here](http://docs.ansible.com/index.html)

[Lostechies.com][1]

[1]: http://lostechies.com
