## This is a read me file

### Generate SSH keys
```
cd ~
ssh-keygen -t rsa
# Above command will generate a private and public SSH keys (RSA encrypted)
# Default path where these get saved is ~/.ssh
# ~/.ssh/id_rsa.pub = public key (copy this into GitHub)
# ~/.ssh/id_rsa = private key (leave this as is)
```

### Copy SSH Keys

**Method 1**
This command copies it to your clip board
```
pbcopy < ~/.ssh/id_rsa.pub
```

**Method 2**
This command will print the file contents in your terminal
Copy this manually with your mouse
```
cat id_rsa.pub
```

### UPload SSh keys to github

1. Go to Settings
2. Go to tab with word "security" or "keys" on it
3. Click on Add
4. Give your SSH keys a title (e.g. name of ur computer), and paste the SSH keys on there
5. Save

### Clone repo to PC

Get SSH url from your github website repo
Select SSH tab and copy the link it gives you
```
cd ~
mkdir repos
cd repos
git clone <ssh-url>
```
