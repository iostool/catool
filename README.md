# Cartool
Cartfile 语法和Carthage大致一样。现在不支持private。简单粗暴.支持多级嵌套Cartfile。特别适合组件开发，新增了package产生，通过-t可以切换到package模式
> **Sample:**
> 
>-  **github "izouxv/gRPC_FMWK"**   *#this is comment,  master will be default branch*
>-  **github "izouxv/gRPC_FMWK" "v1.0.0"** *#this Specify branch as v1.0.0* 
>-  **git "ssh://git@fish.red/fish/test.git"**  *#this is your private git. prefix of github are all public git, if you have private git, you MUST be start with **git "ssh://git@github.com"***
>-  **github "izouxv/gRPC_FMWK" "v1.0.0" "http://xxx.com/gRPC_FMWK.framework.zip"** *#this is release package*

## update
>- **cartool update** will fetch and clone git
>- **cartool update -t** will wget package
 
## build  
>- **cartool build** will clone and build
>- **cartool build -t** will wget package and build 


