<template>
  <div class="page-home" ref="canvas">
    <canvas id="noVNC_canvas" width="800" height="600">
      Canvas not supported.
    </canvas>
  </div>
</template>
<script>
import WebUtil from './../../../../../static/noVnc/app/webutil.js'
import Base64 from './../../../../../static/noVnc/core/base64.js'
import Websock from './../../../../../static/noVnc/core/websock.js'
import './../../../../../static/noVnc/core/des.js'
import './../../../../../static/noVnc/core/input/keysymdef.js'
import './../../../../../static/noVnc/core/input/xtscancodes.js'
import './../../../../../static/noVnc/core/input/util.js'
// import { Keyboard, Mouse } from './../../../../../static/noVNC/core/input/devices.js'
import Display from './../../../../../static/noVnc/core/display.js'
import './../../../../../static/noVnc/core/inflator.js'
import RFB from './../../../../../static/noVnc/core/rfb.js'
import './../../../../../static/noVnc/core/input/keysym.js'
export default {
  data() {
    return {}
  },
  mounted() {}
  // methods: {
  //   // 远程桌面连接成功后的回调函数
  //   _onCompleteHandler(rfb, fbu) {
  //     // 清除 onComplete 的回调。
  //     rfb.set_onFBUComplete(function() {})

  //     var oDisplay = rfb.get_display(),
  //       nWidth = oDisplay.get_width(),
  //       nHeight = oDisplay.get_height(),
  //       oView = oDisplay.get_target(),
  //       nViewWidth = oView.clientWidth,
  //       nViewHeight = oView.clientHeight

  //     // 设置当前与实际的比例。
  //     oDisplay.setScale(nWidth / nViewWidth, nHeight / nViewHeight)
  //   },
  //   _disconnected() {},
  //   connectVNC() {
  //     var DEFAULT_HOST = '',
  //       DEFAULT_PORT = '',
  //       DEFAULT_PASSWORD = '',
  //       DEFAULT_PATH = 'websockify'
  //     var cRfb = null
  //     var oTarget = document.getElementById('noVNC_canvas')
  //     let that = this
  //     if (!this.currentEquipment) {
  //       return
  //     }
  //     // let novncPort = this.currentEquipment.novncPort
  //     WebUtil.init_logging(WebUtil.getConfigVar('logging', 'warn'))
  //     var sHost = '10.202.66.13' || DEFAULT_HOST,
  //       nPort = '5902' || DEFAULT_PORT,
  //       sPassword = DEFAULT_PASSWORD,
  //       sPath = DEFAULT_PATH
  //     cRfb = new RFB({
  //       target: oTarget,
  //       focusContainer: top.document, // 鼠标焦点定位
  //       encrypt: WebUtil.getConfigVar(
  //         'encrypt',
  //         window.location.protocol === 'https:'
  //       ),
  //       repeaterID: WebUtil.getConfigVar('repeaterID', ''),
  //       true_color: WebUtil.getConfigVar('true_color', true),
  //       local_cursor: WebUtil.getConfigVar('cursor', true),
  //       shared: WebUtil.getConfigVar('shared', true),
  //       view_only: WebUtil.getConfigVar('view_only', false),
  //       onFBUComplete: that._onCompleteHandler, // 回调函数
  //       onDisconnected: that._disconnected // 断开连接
  //     })
  //     // console.log('sHost:' + sHost + '--nPort:' + nPort)
  //     cRfb.connect(sHost, nPort, sPassword, sPath)
  //     getNovncIp().then(function(resData) {
  //       WebUtil.init_logging(WebUtil.getConfigVar('logging', 'warn'))
  //       var sHost = resData.data.content.ip || DEFAULT_HOST,
  //         nPort = novncPort || DEFAULT_PORT,
  //         sPassword = DEFAULT_PASSWORD,
  //         sPath = DEFAULT_PATH
  //       cRfb = new RFB({
  //         target: oTarget,
  //         focusContainer: top.document, // 鼠标焦点定位
  //         encrypt: WebUtil.getConfigVar(
  //           'encrypt',
  //           window.location.protocol === 'https:'
  //         ),
  //         repeaterID: WebUtil.getConfigVar('repeaterID', ''),
  //         true_color: WebUtil.getConfigVar('true_color', true),
  //         local_cursor: WebUtil.getConfigVar('cursor', true),
  //         shared: WebUtil.getConfigVar('shared', true),
  //         view_only: WebUtil.getConfigVar('view_only', false),
  //         onFBUComplete: that._onCompleteHandler, // 回调函数
  //         onDisconnected: that._disconnected // 断开连接
  //       })
  //       // console.log('sHost:' + sHost + '--nPort:' + nPort)
  //       cRfb.connect(sHost, nPort, sPassword, sPath)
  //     })
  //   }
  // }
}
</script>