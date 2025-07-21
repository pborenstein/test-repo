20 Jul 2025

In an attempt to get rid of LFS on the amoxtli. I just:

- backed up `/Users/philip/Library/Mobile Documents/iCloud~md~obsidian/Documents/amoxtli` to `/Users/philip/Library/Mobile Documents/iCloud~md~obsidian/Documents/amoxtli-backup-072`0
- removed the .git directory from amoxtli
- create a blank repo on GitHub amoxtli2

```bash
[main =]$ echo "# amoxtli2" >> README.md
		  git init
		  git add README.md
		  git commit -m "Make it so once more"
		  git branch -M main
		  git remote add origin git@github.com:pborenstein/amoxtli2.git
		  git push -u origin main
[main =]$ git add .
[main =]$ git ci -am 'A brand new repo'
[main =]$ git push
```

## Where we are now:

- The amoxtli vault lives canonically on iCloud at:
   `/Users/philip/Library/Mobile Documents/iCloud~md~obsidian/Documents/amoxtli`
- The backup store for the vault is now the GitHub repo: [pborenstein/amoxtli2](https://github.com/pborenstein/amoxtli2)
- The old repo `amoxtli-vault` had to be deleted because that seems to be the only way to remove LFS, which is actually a GitHub thing, not a Git thing, which should have tipped me off not to use it. :shrug:
- The contents of the old repo, with its original git-lfs-infested `.git` directory, lives on at `/Users/philip/Library/Mobile Documents/iCloud~md~obsidian/Documents/amoxtli-backup-0720` The main reason to keep it is for historical data before 20 Jul 2025