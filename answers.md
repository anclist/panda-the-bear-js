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

5.

var highLightItems = document.querySelectorAll('.highlight')
undefined
highLightItems.length
8
highLightItems
(8) [aside.highlight, h1.highlight, div#sleep.bar-filled.highlight, div#eat.bar-filled.highlight, div#time-travel.bar-filled.highlight, div#cry.bar-filled.highlight, h2.highlight, h2.highlight]
for (var i = 0; i < highLightItems.length; i++) {
  highLightItems[i].style.color = 'blue'    
}
"blue"

6.

var h1 = document.querySelector('h1')
undefined
h1
<h1 class=​"highlight" style=​"color:​ blue;​">​Panda The Bear​</h1>​
h1.style.fontFamily = 'monospace'
"monospace"

7.

var actionIcons = document.querySelectorAll('.action-icon i')
undefined
actionIcons
(2) [i.icon-download-alt, i.icon-envelope]
for (var i = 0; i < actionIcons.length; i++) {
  actionIcons[i].style.color = 'grey'    
}
"grey"

8.

var formName = document.querySelector('#name')
undefined
formName
<input type=​"text" name=​"name" class=​"contact-info" id=​"name" placeholder=​"Name">​
formName.placeholder = "identify yourself"
"identify yourself"

9.

var formMessage = document.querySelector('#message')
undefined
formMessage
<textarea name=​"message" id=​"message" placeholder=​"Message">​</textarea>​
formMessage.placeholder = "state your business"
"state your business"

10.

formName.value = "your nemesis"
"your nemesis"
