---
layout: default
title: 本站热点
---

<article class="single row gutters">
  <h2>{{ page.title }}</h2>
  
  <h3>热评文章</h3>
  <!-- 多说热评文章 start -->
	<div class="ds-top-threads" data-range="monthly" data-num-items="5"></div>
  <!-- 多说热评文章 end -->
  
  <h3>最新评论</h3>
  <!-- 多说最新评论 start -->
	<div class="ds-recent-comments" data-num-items="10" data-show-avatars="1" data-show-time="1" data-show-title="1" data-show-admin="1" data-excerpt-length="70"></div>
  <!-- 多说最新评论 end -->

</article>

<!-- 多说公共JS代码 start (一个网页只需插入一次) -->
<script type="text/javascript">
var duoshuoQuery = {short_name:"tegabyte"};
	(function() {
		var ds = document.createElement('script');
		ds.type = 'text/javascript';ds.async = true;
		ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
		ds.charset = 'UTF-8';
		(document.getElementsByTagName('head')[0] 
		 || document.getElementsByTagName('body')[0]).appendChild(ds);
	})();
	</script>
<!-- 多说公共JS代码 end -->