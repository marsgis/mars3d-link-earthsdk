# Mars3D兼容使用earthSDK平台示例

 我们认为，三维SDK平台不是零和游戏，欢迎结合各平台优点，来实现自己的项目需求。该仓库主要实现的就是使用[earthSDK平台](https://www.earthsdk.com)和 [Mars3D](http://cesium.marsgis.cn)结合来实现项目需求。

  该项目运行后效果是的最简应用的创建三维地球项目模版。
   

  其他技术栈，请参考 [Mars3D开源导航](https://github.com/marsgis/MarsGIS-for-Cesium)


## earthSDK整理及修改说明
1. 在[earthSDK官网](https://www.earthsdk.com)下载最新类库，将earthSDK的`XbsjCesium`和`XbsjEarth`等目录拷贝到 `lib\cesiumjs\`目录下；当前示例中地址使用的是earthsdk官方js。
2. 通过earthSDK构造后，使用 viewer.mars=new mars3d.ViewerEx 绑定mars3d的相关处理。




## 使用说明
 在任意开发编辑器（如vscode等）或http服务器(如node、nginx、tomcat、IIS等)下直接运行浏览index.html即可



### 压缩及混淆
 build整站压缩及混淆：[https://github.com/muyao1987/web-dist](https://github.com/muyao1987/web-dist)

 

  
 ## 版权说明
1. 当前[Mars3D](http://cesium.marsgis.cn)免费版本（即`lib/cesiumjs/mars3d/`）可以免费无限制使用.
2. 如有更高需求或商业应用，请联系购买[火星科技](http://cesium.marsgis.cn)进行SDK授权(去除logo、添加授权信息等)。 

