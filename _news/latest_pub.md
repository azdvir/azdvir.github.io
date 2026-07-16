---
layout: post
date: 2099-12-31 00:00:00-0000
inline: true
---
<span id="news-latest-pub">📄 <a href="/publications/">Latest publication</a></span>
<script>
fetch('/publications/').then(function(r){return r.text();}).then(function(html){
  var doc=new DOMParser().parseFromString(html,'text/html');
  var titleEl=doc.querySelector('.title')||doc.querySelector('ol.bibliography li div[class*="title"]')||doc.querySelector('ol li .title');
  var el=document.getElementById('news-latest-pub');
  if(el&&titleEl){
    var yearMatch=(doc.querySelector('h2.year')||{}).textContent||(titleEl.closest('li')||{innerText:''}).innerText.match(/\b(20\d{2})\b/);
    var year=typeof yearMatch==='string'?yearMatch:(yearMatch&&yearMatch[1])||'';
    el.innerHTML='📄 <a href="/publications/" target="_blank">'+titleEl.textContent.trim()+'</a>';
    var th=(el.closest('tr')||{}).querySelector&&el.closest('tr').querySelector('th');
    if(th&&year) th.textContent=year;
  }
}).catch(function(){});
</script>
