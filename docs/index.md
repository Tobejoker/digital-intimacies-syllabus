---
hide:
  #- navigation # 显示右
  #- toc #显示左
  - footer
  - feedback
comments: false
---                               

<div><font  color= #518FC1 size=6 class="ml3">We may have all come on different ships, but we’re in the same boat now.</font></div>
<center><font  color= #518FC1 size=3 class="ml3" style='text-align=right'">- Martin Luther King, Jr.</font></center>
<!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js"></script>-->

<!-- 
<center>
<font  color= #608DBD size=3>
<span id="jinrishici-sentence">正在加载今日诗词....</span>
<script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8"></script>
</font>
</center>
-->

<!-- 可选一言 -->
<!-- <center>
<font  color= #608DBD size=3>
<p id="hitokoto">
  <a href="#" id="hitokoto_text" target="_blank"></a>
</p>
<script>
  fetch('https://v1.hitokoto.cn')
    .then(response => response.json())
    .then(data => {
      const hitokoto = document.querySelector('#hitokoto_text')
      hitokoto.href = `https://hitokoto.cn/?uuid=${data.uuid}`
      hitokoto.innerText = data.hitokoto
    })
    .catch(console.error)
</script>
</font>
</center> -->

<div id="rcorners2" >
  <div id="rcorners1">
    <!-- <i class="fa fa-calendar" style="font-size:100"></i> -->
    <body>
      <font color="#4351AF">
        <p class="p1"></p>
<script defer>
    //格式：2020年04月12日 10:20:00 星期二
    function format(newDate) {
        var day = newDate.getDay();
        var y = newDate.getFullYear();
        var m =
            newDate.getMonth() + 1 < 10
                ? "0" + (newDate.getMonth() + 1)
                : newDate.getMonth() + 1;
        var d =
            newDate.getDate() < 10 ? "0" + newDate.getDate() : newDate.getDate();
        var h =
            newDate.getHours() < 10 ? "0" + newDate.getHours() : newDate.getHours();
        var min =
            newDate.getMinutes() < 10
                ? "0" + newDate.getMinutes()
                : newDate.getMinutes();
        var s =
            newDate.getSeconds() < 10
                ? "0" + newDate.getSeconds()
                : newDate.getSeconds();
        var dict = {
            1: "Monday",
            2: "Tuesday",
            3: "Wednesday",
            4: "Thursday",
            5: "Friday",
            6: "Saturday",
            0: "Sunday",
        };
        //var week=["日","一","二","三","四","五","六"]
        return (
            y +
            "/" +
            m +
            "/" +
            d +
            " " +
            h +
            ":" +
            min +
            ":" +
            s +
            " " +
            dict[day]
        );
    }
    var timerId = setInterval(function () {
        var newDate = new Date();
        var p1 = document.querySelector(".p1");
        if (p1) {
            p1.textContent = format(newDate);
        }
    }, 1000);
</script>
      </font>
    </body>
    <!-- <b><span id="time"></span></b> -->
  </div>
  <ul>
    <li>Access articles through tags or navigation</li>
    <ul>
      <li>Graduate-level seminar</li>
      <li>Emphasis on Gender and Women's Studies</li>
      <li>Developing and collaborative</li>
    </ul>
  </ul>
</div>

<!-- - 基于Material for MkDocs美化
- 简洁美观，功能多元化
- 简单易上手，小白配置
- 𝕙𝕒𝕧𝕖 𝕒 𝕘𝕠𝕠𝕕 𝕥𝕚𝕞𝕖 ! -->

<!-- - 快速谈话(1) 联系我(2)
{ .annotate }

1. 点击右下角与我在线交谈.
2. 18939533255

***   ! -->

<!-- <strong>推荐文章:material-book:</strong>

  - [利用Mkdocs部署静态网页至GitHub pages](blog/Mkdocs/mkdocs1.md)
  - [Mkdocs部署配置说明(mkdocs.yml)](blog/Mkdocs/mkdocs2.md)
  - [如何给MKdocs添加友链](blog/websitebeauty/linktech.md)
  - [网站添加Mkdocs博客](blog/Mkdocs/mkdocsblog.md)
  - [Blogger](blog/index.md) -->

<div class="grid cards" markdown>

- :simple-materialformkdocs:{ .lg .middle } __Quick Links__

    ---
  - [Syllabus](develop/syllabus/basics/week1.md)
  - [Inspirations](about/inspirations.md)
  - [Full bibliography](develop/resources/database.md)
  - [Forthcoming modules](develop/syllabus/topics/index.md)

- :simple-aboutdotme:{ .lg .middle } __About__

    ---
  - [How to use this](about/documentation.md)
  - [Coming next](about/whatnext.md)
  - [Project origin](about/origin.md)

</div>

   <body>
        <font color="#B9B9B9">
        <p style="text-align: center; ">
                <span>The project has started for </span>
                <span id='box1'></span>
    </p>
      <div id="box1"></div>
      <script>
        function timingTime(){
          let start = '2024-11-23 22:46:10 '
          let startTime = new Date(start).getTime()
          let currentTime = new Date().getTime()
          let difference = currentTime - startTime
          let m =  Math.floor(difference / (1000))
          let mm = m % 60  // 秒
          let f = Math.floor(m / 60)
          let ff = f % 60 // 分钟
          let s = Math.floor(f/ 60) // 小时
          let ss = s % 24
          let day = Math.floor(s  / 24 ) // 天数
          return day + " days, " + ss + " hours, " + ff + " minutes, " + mm +' seconds, '
        }
        setInterval(()=>{
          document.getElementById('box1').innerHTML = timingTime()
        },1000)
      </script>
      </font>
    </body>
