# CrednClip
Linux command to clip and use your credentials

## Setup

Copy 'cred' file to your home folder
```
cp cred ~/cred
```

### Linux
Open and edit bashrc file with your favourite text editor
```
nano ~/.bashrc
```

Paste following code to end of the file
```
function cred() {
    sed -n "/$1/,/$1/p" ~/cred
}
```
Save and exit

```
source ~/.bashrc
```

### Mac
Navigate to your home folder
```
cd ~/
```
Create your new file
```
touch .bash_profile
```
Edit .bash_profile with your favorite editor (or you can just type open -e .bash_profile to open it in TextEdit).

Paste following code to end of the file
```
function cred() {
    sed -n "/$1/,/$1/p" ~/cred
}
```
Save and exit

Reload your bash profile and update any alias you add.
```
. .bash_profile
```

## Use

Use cred command to get all the contents inside 'Title1' title
```
cred Title1
```
Update cred file using
```
nano ~/cred
```

