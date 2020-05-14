# Run servers:
1 Generate ssh keys:

- Run command ```ssh-keygen``` in directory ```~/.ssh/```

- Use   ```id_rsa_devops_group4``` as the name

- Leave passphrase empty
  
- Add to the `~/.ssh/config` file on host

```
Host devops-group4-integration-vm
        User vagrant
        Hostname 192.168.80.1  
        IdentityFile ~/.ssh/id_rsa_devops_group4

Host devops-group4-testing-vm
        User vagrant
        Hostname 192.168.80.2
        IdentityFile ~/.ssh/id_rsa_devops_group4

Host devops-group4-production-vm
        User vagrant
        Hostname 192.168.80.3
        IdentityFile ~/.ssh/id_rsa_devops_group4

```

2 Start servers:
- Go to the `/servers/integration/` and run `vagrant up`
- Go to the `/servers/testing/` and run `vagrant up`
- Go to the `/servers/production/` and run `vagrant up`

testtttttt
