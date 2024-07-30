---
layout: page
permalink: /blogs/index.html
title: Blogs
---
### Today

 <script>
        Date.prototype.format = function (fmt) {
            var o = {
                "y+": this.getFullYear, //年
                "M+": this.getMonth() + 1, //月份
                "d+": this.getDate(), //日
                "h+": this.getHours(), //小时
                "m+": this.getMinutes(), //分
                "s+": this.getSeconds() //秒
            };
            if (/(y+)/.test(fmt)) fmt = fmt.replace(RegExp.$1, (this.getFullYear() + "").substr(4 - RegExp.$1.length));
            for (var k in o)
                if (new RegExp("(" + k + ")").test(fmt)) fmt = fmt.replace(RegExp.$1, (RegExp.$1.length == 1) ? (o[k]) : (("00" + o[k]).substr(("" + o[k]).length)));
            return fmt;
        }
        setInterval("document.getElementById('dateTime').innerHTML = (new Date()).format('yyyy-MM-dd hh:mm:ss');", 1000);
    </script>

---


### 2024

---

#### Leave a Message



{% include disqus.html %} 

<br><br>
<center>
    <script type="text/javascript" src="//widget.supercounters.com/ssl/vt.js"></script>
    <script
        type="text/javascript">var sc_visitor_var = sc_visitor_var || []; sc_vt(1695896, "FFFFFF", "cccccc", "000000", 3)</script>
    <br><noscript><a href="http://www.supercounters.com/">free online counter</a></noscript>
<script type="text/javascript" src="//widget.supercounters.com/ssl/map.js"></script><script type="text/javascript">var sc_map_var = sc_map_var || [];sc_map(1695900,"112288","ff0000",81)</script><br><noscript><a href="http://www.supercounters.com/">free online counter</a></noscript>
</center>















