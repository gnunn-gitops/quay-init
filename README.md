An ansible playbook to initialize the Quay Registry, inspiration and some snippets taken from [RHEL Edge Automation](https://github.com/redhat-cop/rhel-edge-automation-arch) project.

You will need to initialize the modules used from ansible galaxy as follows:

```
ansible-galaxy collection install -r collections/requirements.yml
```

When you run the playbook you can override the variables by passing them in as environment variables, i.e.

```
ansible-playbook init-quay.yaml -e quay_init_password=testing
```