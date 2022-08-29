# ansible roles

> sudo dnf install linux-system-roles

edit settings and

> ansible-playbook nbde.yml -i inventory.yml --ask-vault-pass -b

# gen

> butane --pretty --strict example.bu > example.ign



# pass

```
$ podman run -ti --rm quay.io/coreos/mkpasswd --method=yescrypt
Password:
$y$j9T$A0Y3wwVOKP69S.1K/zYGN.$S596l11UGH3XjN...
```