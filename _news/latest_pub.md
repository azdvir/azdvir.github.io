---
layout: post
date: 2099-12-31 00:00:00-0000
inline: true
---
<span id="news-latest-pub">📄 <a href="/publications/">Loading...</a></span>
<script>
fetch('/publications/').then(function(r){return r.text();}).then(function(html){
  var doc=new DOMParser().parseFromString(html,'text/html');
  var li=doc.querySelector('ol.bibliography li');
  if(!li) return;
  var titleEl=li.querySelector('.title');
  var yearMatch=li.textContent.match(/\b(20\d{2})\b/);
  var el=document.getElementById('news-latest-pub');
  if(el&&titleEl){
    el.innerHTML='📄 <a href="/publications/" target="_blank">'+titleEl.textContent.trim()+'</a>';
    var row=el.closest('tr');
    if(row&&yearMatch) row.querySelector('th').textContent=yearMatch[1];
  }
}).catch(function(){});
</script>
