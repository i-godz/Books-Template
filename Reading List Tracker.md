---
cssclasses:
  - cards
---
<div class="tabbed-container">
  <div class="tab-buttons">
    <button id="tab3" class="tab-button finished">Finished</button>

  </div>
</div>

~~~dataview 
Table ("![](" + cover_url + ")") AS Cover,
total_pages AS Pages, author AS Author
From "Books"
where contains(status, "Finished")
~~~
\
	
<div class="tabbed-container">
  <div class="tab-buttons">
    <button id="tab1" class="tab-button currently-reading">Currently Reading</button>
  </div>
</div> 

~~~dataview 
Table ("![](" + cover_url + ")") AS Cover,
total_pages AS Pages, author AS Author
From "Books Template/Books"
where contains(status, "Reading")
~~~
<div class="tabbed-container">
  <div class="tab-buttons">
    <button id="tab2" class="tab-button unfinished">Unfinished</button>

  </div>
</div>

~~~dataview 
Table ("![](" + cover_url + ")") AS Cover,
total_pages AS Pages, author AS Author
From "Books Template/Books"
where contains(status, "To Read")
~~~


