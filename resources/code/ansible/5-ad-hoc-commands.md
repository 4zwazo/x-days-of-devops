## ansible [pattern] -m [module] -a "[module option]"
## Modules
```
- Ping
- command
- Stat
- Yum
- User
- Setup
```

## Ping ad-hoc command

```
command:
ansible all -m ping

results:
10.0.1.77 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/libexec/platform-python"
    },
    "changed": false,
    "ping": "pong"
}

```