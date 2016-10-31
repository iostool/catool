# cartool
cartool's Cartfile syntax roughly the same as Carthage. Private is not supported right now. it Simple and crude.it Support for multi-level nested Cartfile. Particularly suitable for component development, use **-p** can switch to the package mode

> **Sample:**
> 
>-  **github "izouxv/gRPC_FMWK"**   *#this is comment,  master will be default branch*
>-  **github "izouxv/gRPC_FMWK" "v1.0.0"** *#this Specify branch as v1.0.0* 
>-  **git "ssh://git@fish.red/fish/test.git"**  *#this is your private git. prefix of github are all public git, if you have private git, you MUST be start with **git "ssh://git@github.com"***
>-  **github "izouxv/gRPC_FMWK" "v1.0.0" "http://xxx.com/gRPC_FMWK.framework.zip"** *#this is release package*

## update
>- **cartool update** will fetch and clone git
>- **cartool update -p** will wget package
 
## build  
>- **cartool build** will clone and build
>- **cartool build -p** will wget package and build 

## archive  
>- **cartool archive** archive all package
>- **cartool archive -t** archive current package 

## cmd sample  
>- **cartool update && cartool build && cartool archive**
>- **cartool update -p && cartool build -p && cartool archive**
