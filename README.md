# Mars3D兼容使用earthSDK使用示例

 我们认为，三维SDK平台不是零和游戏，欢迎结合各平台优点，来实现自己的项目需求。该仓库主要实现的就是使用[earthSDK平台](https://www.earthsdk.com)和 [Mars3D](http://cesium.marsgis.cn)结合来实现项目需求。

  该项目运行后效果是的最简应用的创建三维地球项目模版。
   

  其他技术栈，请参考 [Mars3D开源导航](https://github.com/marsgis/MarsGIS-for-Cesium)


## earthSDK整理及修改说明
1. 将earthSDK的`XbsjCesium`和`XbsjEarth`等目录拷贝到 `lib\cesiumjs\`目录下；
	
2. 修改lib\cesiumjs\XbsjEarth\XbsjEarth.js文件的`function ready()`方法，
	将`loadCesium().then(loadXbsjCesium).then(loadViewerCesiumNavigationMixin)`代码删除，因为在`lib\include-lib.js`中配置加载,修改后代码为；
```javascript
function ready() {
    //调试模式下
    if (false) {
        return loadRxjs().then(function () {
            return ready.isReady = true;
        });
    } else {
        // 同时加载尽可能多的js包，已提升加载速度！
        return _promise2.default.all([loadRxjs()]).then(function () {
            return ready.isReady = true;
        });
    }
}
```

3. 通过earthSDK构造后，使用 viewer.mars=new mars3d.ViewerEx 绑定mars3d的相关处理。




## 使用说明
 在任意开发编辑器（如vscode等）或http服务器(如node、nginx、tomcat、IIS等)下直接运行浏览index.html即可



### 压缩及混淆
 build整站压缩及混淆：[https://github.com/muyao1987/web-dist](https://github.com/muyao1987/web-dist)

 

  
 
## 版权说明
  本项目主要是为了展示[Mars3D](http://cesium.marsgis.cn)的项目应用，仅限大家学习之用，如需用于商业项目，请联系购买[火星科技](http://cesium.marsgis.cn)SDK授权。
 并且Mars3D-SDK类库并未开源（即`libs/cesiumjs/mars3d/`）,在线演示版内部有作者公司logo及时效限制。