# CrednClip
Linux command to clip and use your credentials

## Setup
```
nano ~/.bashrc
```

```
function cred() {
    sed -n "/$1/,/$1/p" ~/cred
}
```

```
source ~/.bashrc
```

## Use
```
cred <title>
```

