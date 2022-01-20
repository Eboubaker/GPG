# GPG
My GPG Keys Index
## Personal GPG Key
encrypt stuff or check signature with this key.
```
# import directly from github
curl https://github.com/Eboubaker.gpg | gpg --import
# import from keyserver
gpg --keyserver keyserver.ubuntu.com --recv-key 967057A0
```

# Footer
some used commands
```
gpg --full-generate-key
gpg --list-secret-keys --keyid-format=long
gpg --armor --export XXXXXXXXXX


# Force git to use GPG
git config --global gpg.program "/path/to/gpg"
git config --global user.signingkey XXXXXXXXXXX
git config --global commit.gpgsign true
git config --global commit.gpgSign true
git config --global user.email "eboubakkar@gmail.com"
git config --global user.name "Eboubaker Bekkouche"


## Export all public keys
gpg -a --export >mypubkeys.asc
## Export all encrypted private keys (which will also include corresponding public keys)
gpg -a --export-secret-keys >myprivatekeys.asc


#delete GPG key
gpg --delete-secret-keys XXXXXXXXXXXXXXXXX
gpg --delete-key XXXXXXXXXXXXXX

```
