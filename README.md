# GPG
My GPG Keys Index
# GPG Keys
## GitHub
#### My VPS GPG key
```
Key ID: EA7015980A99803E
Subkeys: 834ACEF983DEE193
Added on Jan 19, 2022
```
```
sec   rsa4096/EA7015980A99803E 2022-01-19 [SC] [expires: 2023-01-19]
      A51E44086B647D60161808E0EA7015980A99803E
uid                 [ultimate] Eboubaker Bekkouche (My VPS GPG key) <eboubakkar@gmail.com>
ssb   rsa4096/834ACEF983DEE193 2022-01-19 [E] [expires: 2023-01-19]
```
#### Work GPG key
```
Key ID: 22DFCECD1810037B
Subkeys: A471F373C23F4DD6
Added on Jan 19, 2022
```
```
sec   rsa4096/22DFCECD1810037B 2022-01-19 [SC] [expires: 2022-07-18]
      DEA231734D6BCB16D56A757322DFCECD1810037B
uid                 [ultimate] Eboubaker Bekkouche (Work GPG Key) <eboubakkar@gmail.com>
ssb   rsa4096/A471F373C23F4DD6 2022-01-19 [E] [expires: 2022-07-18]
```


# Footer
```
gpg --full-generate-key
gpg --list-secret-keys --keyid-format=long
gpg --armor --export XXXXXXXXXX


# Force git to use GPG
git config --global gpg.program "/path/to/gpg"
git config --global user.signingkey XXXXXXXXXXX
git config --global commit.gpgsign true
git config --global commit.gpgSign true

## Export all public keys
gpg -a --export >mypubkeys.asc
## Export all encrypted private keys (which will also include corresponding public keys)
gpg -a --export-secret-keys >myprivatekeys.asc


#delete GPG key
gpg --delete-secret-keys XXXXXXXXXXXXXXXXX
gpg --delete-key XXXXXXXXXXXXXX

```
