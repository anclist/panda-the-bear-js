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

11.

var formEmail = document.querySelector('#email')
undefined
formEmail.value = "koalathebear@gmail.com"
"koalathebear@gmail.com"

12.

var formButton = document.querySelector('#submit')
undefined
formButton.value = "En garde!"
"En garde!"

13.

formButton.disabled = true
true
formButton
<input type=​"submit" name=​"submit" id=​"submit" value=​"En garde!" disabled>​

14.

var personalInfo = document.querySelector('.bio-info')
undefined
var personalInfoItems = document.querySelectorAll('.bio-info li')
undefined
for (var i = 0; i < personalInfoItems.length; i++) {
  personalInfo.removeChild(personalInfoItems[i]);  
}
<li class=​"bio-info-item">​…​</li>​<span class=​"bio-info-title">​Phone​</span>​<span class=​"bio-info-value bio-info-phone">​555 123 1234​</span>​</li>​
personalInfo
<ul class=​"bio-info">​</ul>​

__________________________________________________

Day 2

Removing Elements from the DOM

1.

var timeTravelBar = $('#time-travel').parent('.bar-default')
undefined
timeTravelBar.remove()
[div.bar-default, prevObject: n.fn.init(1), context: document]

Adding Elements to the DOM

1 & 2.

var container = document.querySelector('.portfolio-container')
undefined
for (var i = 0; i < 10; i++) {
  var picachuClone = document.querySelector('#right-image').cloneNode(true)
  container.appendChild(picachuClone)
}
<div class=​"portfolio-image" id=​"right-image">​…​</div>​

3.

var listItem = document.createElement('li');
listItem.className = "bio-info-item";
listItem
var leftSpan = document.createElement('span');
leftSpan.className = "bio-info-title";
leftSpan
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
listItem
var rightSpan = document.createElement('span');
rightSpan.className = "bio-info-value bio-info-updated-at";
"bio-info-value bio-info-updated-at"
var dateNow = document.createTextNode(new Date());
undefined
dateNow
"Fri Nov 10 2017 15:20:40 GMT-0500 (EST)"
rightSpan.appendChild(dateNow)
"Fri Nov 10 2017 15:20:40 GMT-0500 (EST)"
listItem.appendChild(rightSpan);
<span class=​"bio-info-value bio-info-updated-at">​Fri Nov 10 2017 15:20:40 GMT-0500 (EST)​</span>​
listItem
<li class=​"bio-info-item">​<span class=​"bio-info-title">​Page last updated on​</span>​<span class=​"bio-info-value bio-info-updated-at">​Fri Nov 10 2017 15:20:40 GMT-0500 (EST)​</span>​</li>​
var ulItem = document.querySelector('.bio-info')
undefined
ulItem
<ul class=​"bio-info">​…​</ul>​
ulItem.appendChild(listItem)
<li class=​"bio-info-item">​…​</li>​
