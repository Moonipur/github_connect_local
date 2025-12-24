# github_connect_local

1. Check Existing SSH Keys
```
ls -al ~/.ssh
```

2. Generate a New SSH Key (Recommended: ed25519)
```
ssh-keygen -t ed25519 -C "your.email@example.com"
```

3. Add SSH Public Key to GitHub
```
cat ~/.ssh/id_ed25519.pub
```

4. Test SSH Connection to GitHub
```
ssh -T git@github.com
```

5. Use SSH with Git Repositories
```
git clone git@github.com:USERNAME/REPOSITORY.git
git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
git remote -v
```

