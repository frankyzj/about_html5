利用 

### 格式问题 {#格式问题}

| 格式 | 说明 | 扩展名 | MIME类型 |
| :--- | :--- | :--- | :--- |
| MP3 | 有使用许可费 | .mp3 | audio/mp3 |
| Ogg Vorbis | 免费、开放 | .ogg | audio/ogg |
| H.264 | 视频压缩行业标准，收费 | .mp4 | video/mp4 |
| Ogg Theora | 免费、开放，品质和性能稍差 | .ogv | video/ogg |
| WebM | Google 支持，免费 | .webm | video/webm |
| WAV | 未压缩 | .wav | audio/wav |

```
* MIME 类型表示某种 Web 资源的内容类型。

```

以上为 Web 中常见的音频和视频格式。

* 一个视频文件实际上有三个标准参与其中：视频编解码器；音频编解码器；容器（把视频、音频、描述性信息和静态图片、字幕等组合到一起）的格式。

#### 使用 &lt;source&gt; 元素支持多种格式 {#使用-source-元素支持多种格式}

```
<
video controls width="400" height="300"
>
<
source src="discoParty.mp4" type="video/mp4"
>
<
source src="discoParty.ogv" type="video/ogg"
>
<
p
>
We like disco dancing.
<
/p
>
<
/video
>
```

#### 一个支持 flash 播放器 flowplayer 的例子 {#一个支持-flash-播放器-flowplayer-的例子}

```
<
video controls width="700" height="400"
>
<
source src="beach.mp4" type="videa/mp4" /
>
<
source src="beach.ogv" type="videa/ogv" /
>
<
object id="flowplayer" width="700" height="400"
        data="flowplayer-3.2.7.swf"
        type="application/x-shockwave-flash"
>
<
param name="movie" value="flowplayer-3.2.7.swf"
>
<
param name="flashvars" value="config={"clip":"beach.mp4"}"
>
<
/object
>
<
/video
>
```



