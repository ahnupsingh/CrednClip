# CrednClip
Linux command to clip and use your credentials

## Setup

Copy 'cred' file to your home folder
```
cp cred ~/cred
```

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

## Use

Use cred command to get all the contents inside 'Title1' title
```
cred Title1
```

