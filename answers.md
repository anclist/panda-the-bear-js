1.

var pandaImage = document.querySelector('.profile-image')
undefined
pandaImage
<img src=​"images/​self-portrait-grassbg.jpg" alt=​"Self Portrait" title=​"Self Portrait" class=​"profile-image">​
pandaImage.src = "http://www.3drivers.com/upload/iblock/799/panda_tuy-c-0000.jpg"
"http://www.3drivers.com/upload/iblock/799/panda_tuy-c-0000.jpg"

2.

var mainTitle = document.querySelector('h1')
undefined
mainTitle
<h1 class=​"highlight">​Panda The Bear​</h1>​
mainTitle.innerText = "Antonio Manzanares"
"Antonio Manzanares"

3.

var icon = document.querySelector('#employment h3 i')
undefined
var workHistory = document.createElement("span")
undefined
workHistory.innerHTML = "&nbsp; Work History"
"&nbsp; Work History"
var employmentHeading = document.querySelector('#employment h3')
undefined
employmentHeading.innerText = ""
""
employmentHeading.appendChild(icon)
<i class=​"icon-suitcase">​…​</i>​
employmentHeading.appendChild(workHistory)
<span>​&nbsp; Work History​</span>​


4.

var body = document.querySelector('body')
undefined
body.style.backgroundColor = "red"
"red"
