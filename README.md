# Flux APT repository.

Use the following to set it up. 
```
echo 'deb https://apt.runonflux.io/ '$(lsb_release -cs)' main' | sudo tee --append /etc/apt/sources.list.d/flux.list
gpg --keyserver keyserver.ubuntu.com --recv 4B69CA27A986265D
gpg --export 4B69CA27A986265D | sudo apt-key add -

sudo apt-get update
sudo apt-get install flux # to install Flux daemon
sudo apt-get install fluxbench # to install Flux benchmark
sudo apt-get install zelcore # to install Zelcore
```

## Available Packages

### amd64
```
flux
        Depends: libc6 (&gt;= 2.17), libgcc1 (&gt;= 1:3.0), libgomp1 (&gt;= 4.9), libstdc++6 (&gt;= 5.2)

fluxbench
        Depends: libc6 (&gt;= 2.17), libgcc1 (&gt;= 1:3.0), libgomp1 (&gt;= 4.9), libstdc++6 (&gt;= 5.2)

zelcore
        Depends:
```


### arm64
```
flux
        Depends: libc6 (&gt;= 2.17), libgcc1 (&gt;= 1:3.0), libgomp1 (&gt;= 4.9), libstdc++6 (&gt;= 5.2)
        
fluxbench
        Depends: libc6 (&gt;= 2.17), libgcc1 (&gt;= 1:3.0), libgomp1 (&gt;= 4.9), libstdc++6 (&gt;= 5.2)
```
