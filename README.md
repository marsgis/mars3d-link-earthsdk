# Mars3D最简项目模版 - EarthSDK版
  Mars3D支持结合`Cesium相关的各类平台`来兼容使用，方便结合不同平台的优点来达到完成各种项目需求。
   
  本仓库是Mars3D三维地球平台软件，在北京西部世界公司[EarthSDK平台](https://www.earthsdk.com)技术栈下的最简的应用项目模版。
  

 > 其他技术栈，请参考： [https://github.com/marsgis/mars3d](https://github.com/marsgis/mars3d)

  

### EarthSDK整理及修改说明
1. 在[EarthSDK官网](https://www.earthsdk.com)下载最新类库，将earthSDK的`XbsjCesium`和`XbsjEarth`等目录拷贝到 `lib\`目录下；当前示例中地址使用的是earthsdk官方js。
2. 通过earthSDK构造后，使用 `new mars3d.Map(viewer, mapOptions)` 绑定mars3d的相关处理。



 
## 运行站点
 在任意开发编辑器（如vscode等）或http服务器(如node、nginx、tomcat、IIS等)下直接运行浏览index.html即可



## 压缩及混淆
 如果需要编译、对整站压缩及混淆，请参考：[https://github.com/muyao1987/web-dist](https://github.com/muyao1987/web-dist)

 



## Mars3D 是什么 
> `Mars3D三维地球平台软件` 是[火星科技](http://marsgis.cn/)团队研发的二三维一体的WebGIS地图开发平台，是火星科技团队成员多年GIS开发和Cesium使用的技术沉淀。基于[Cesium](https://cesium.com/cesiumjs/)开源库和现代Web技术栈全新构建，该平台框架优化了Cesium的使用方式和增添了更多高级功能。集成了领先的开源地图库、可视化库，提供了全新的三维大数据可视化、实时流数据可视化功能，通过本产品可快速实现浏览器和移动端上美观、流畅的三维地图呈现与空间分析。

### 相关网站 
- Mars3D官网：[http://mars3d.cn](http://mars3d.cn)  

- GitHub导航列表：[https://github.com/marsgis/mars3d](https://github.com/marsgis/mars3d)


## 版权说明
1. 任何`个人或组织`可以在遵守Mars3D相关要求下`免费无限制`使用。
2. 如有`个性化需求`或`商业应用`，请联系[火星科技](http://mars3d.cn)购买。