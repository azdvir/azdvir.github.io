---
layout: post
date: 2099-12-30 00:00:00-0000
inline: true
---
<span id="news-linkedin-personal">🔗 <a href="https://www.linkedin.com/in/amit-dvir-b3111b7/" target="_blank">Loading...</a></span>
<script>
fetch('https://rss.app/feeds/v1.1/MyCmjZ0TVFeGLzgA.json').then(function(r){return r.json();}).then(function(data){
  var item=data.items&&data.items[0];
  var el=document.getElementById('news-linkedin-personal');
  if(el&&item){
    var d=new Date(item.date_published);
    var ds=d.toLocaleDateString('en-US',{month:'short',year:'numeric'});
    el.innerHTML='🔗 <a href="'+(item.url||'#')+'" target="_blank">'+(item.title||'LinkedIn post')+'</a>';
    var row=el.closest('tr');
    if(row) row.querySelector('th').textContent=ds;
  }
}).catch(function(){});
</script>
