## 使用 JavaScript 控制播放器 {#使用-javascript-控制播放器}

* &lt;
  audio
  &gt;
   和 
  &lt;
  video
  &gt;
   都有一个扩展的 JavaScript 对象模型。

### 添加音效 {#添加音效}

开始音效：

```
var audioElement = document.getElementById("backgroundMusic");
audioElement.play();

```

停止音效：

```
var audioElement = document.getElementById("backgroundMusic");
audioElement.pause();
audioElement.currentTime = 0;

```

#### 控制播放 {#控制播放}

* playbackRate 用来控制视频播放速度。

```
video.play();
video.playbackRate = 0.5;//0.5倍速播放，设为 ?1 则会倒退播放。

```

* 视频播放过程中，
  &lt;
  video
  &gt;
   元素会连续触发 onTimeUpdate 元素，进而可以更新播放进度条。

  


