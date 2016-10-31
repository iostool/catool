# Cartool

Cartfile 语法和Carthage的一样。现在不支持private。简单粗暴.支持多级嵌套Cartfile。特别适合组件开发
 
//update
#'cartool update'  will fetch and clone git
github "izouxv/gRPC_FMWK" "v1.0.0"    

#'cartool update' will fetch and clone git
#'cartool update -t' will wget package
github "izouxv/gRPC_FMWK" "v1.0.0" "http://xxx.com/gRPC_FMWK.framework.zip"  


//build 
#'cartool build' // will clone and build
github "izouxv/gRPC_FMWK" "v1.0.0"    

#'cartool build' will clone and build
#'cartool build -t' will wget and build
github "izouxv/gRPC_FMWK" "v1.0.0" "http://xxx.com/gRPC_FMWK.framework.zip"  
