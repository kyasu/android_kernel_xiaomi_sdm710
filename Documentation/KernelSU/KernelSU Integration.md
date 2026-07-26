# KernelSU Integration

> '''
>
> * #### The official KSU has not supported `non-gki` devices for a long time.
>
> * #### So we chose the more reliable KSU fork.
>
> '''

### Backslashxx's KernelSU
---------------------------------

> '''
> 
> * [Repository](https://github.com/backslashxx/KernelSU)
> * [Releases](https://github.com/backslashxx/KernelSU/releases)
> 
> '''

### ReSukiSU
---------------------------------

> '''
> 
> * [Repository](https://github.com/ReSukiSU/ReSukiSU)
> * [Releases](https://t.me/ReSukiSU/4)
> 
> '''

### How To Setup
---------------------------------

```shell
# 1. into workdir
cd android_kernel_xiaomi_sdm710

# 2. setup with KernelSU
# xxksu
curl -LSs https://raw.githubusercontent.com/backslashxx/KernelSU/master/kernel/setup.sh  | bash -s master
# or resuki
curl -LSs https://raw.githubusercontent.com/ReSukiSU/ReSukiSU/main/kernel/setup.sh  | bash -s main
```

### Quick Build (Github Actions)
---------------------------------

> '''
> 
> 1. fork this repository
> 
> 2. enable github actions
>
> 3. create a repository's secret of actions (optional)
>
>    name: `SIGNING_KEY`
>
>    content: like `certs/signing_key.pem`
>
>             -----BEGIN PRIVATE KEY-----
>             MIIJQw...more content...0zxuI=
>             -----END PRIVATE KEY-----
>             -----BEGIN CERTIFICATE-----
>             MIIFKD...more content...R8gw==
>             -----END CERTIFICATE-----
> 
> 4. manual run workflow (Build Kernel With KernelSU)
>
> '''

### Related
---------------------------------

> '''
>
> * [xxksu: scope-minimized manual hooks](https://github.com/backslashxx/KernelSU/issues/5)
>
> * [resuki: manual-integrate](https://resukisu.github.io/guide/manual-integrate.html)
> 
> '''
