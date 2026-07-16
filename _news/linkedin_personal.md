---
layout: post
date: 2099-12-30 00:00:00-0000
inline: true
---
<span id="news-linkedin-personal">🔗 <a href="https://www.linkedin.com/in/amit-dvir-b3111b7/" target="_blank">Latest LinkedIn post loading...</a></span>
<script>
fetch('https://rss.app/feeds/v1.1/MyCmjZ0TVFeGLzgA.json')
  .then(function(r){return r.json();})
  .then(function(data){
    var item=data.items&&data.items[0];
    var el=document.getElementById('news-linkedin-personal');
    if(el&&item){
      var title=item.title||'Latest LinkedIn post';
      var url=item.url||'https://www.linkedin.com/in/amit-dvir-b3111b7/';
      el.innerHTML='🔗 <a href="'+url+'" target="_blank">'+title+'</a>';
    }
  }).catch(function(){});
</script>
