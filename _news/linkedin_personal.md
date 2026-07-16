---
layout: post
date: 2099-12-30 00:00:00-0000
inline: true
---
<span id="news-linkedin-personal">🔗 <a href="https://www.linkedin.com/in/amit-dvir-b3111b7/" target="_blank">Latest LinkedIn post</a></span>
<script>
var proxy='https://api.rss2json.com/v1/api.json?rss_url=';
var feed=encodeURIComponent('https://rss.app/feeds/MyCmjZ0TVFeGLzgA.xml');
fetch(proxy+feed).then(function(r){return r.json();}).then(function(data){
  var item=data.items&&data.items[0];
  var el=document.getElementById('news-linkedin-personal');
  if(el&&item){
    var d=new Date(item.pubDate);
    var ds=d.toLocaleDateString('en-US',{month:'short',year:'numeric'});
    el.innerHTML='🔗 <a href="'+(item.link||'#')+'" target="_blank">'+(item.title||'LinkedIn post')+'</a>';
    var th=el.closest('tr')&&el.closest('tr').querySelector('th');
    if(th) th.textContent=ds;
  }
}).catch(function(){});
</script>
