# Mac Provisioning
```commandline
xcode-select --install

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install ansible

git clone https://github.com/iskrmky/mac.git

ansible-playbook -i inventory/localhost localhost.yml --ask-become-pass --ask-vault-pass
```

## Note
Delete Pycharm data
```commandline
find ~/Library -iname "*pycharm*" -exec rm -r "{}" \;
```

Decrypt secret file
```commandline
ansible-vault decrypt secret.yml
```

Encrypt secret file
```commandline
ansible-vault encrypt secret.yml
```
