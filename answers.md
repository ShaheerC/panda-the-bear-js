# PART 1 

# 1.1 
- In console type document
- let newImg = document.querySelector('.profile-mage')
- newImg.src = "https://placebear.com/400/400"

# 1.2
- let skyImg = document.querySelector('#left-image > img')
- skyImg.src = "https://picsum.photos/id/188/325/225"

# 2
- let topTitle2 = document.querySelector('div > .highlight')
- topTitle2.innerText = "Shaheer Choudhury"

# 3
- let employment = document.querySelector('#employment > .info-title')
- employment.innerText = "Experience"

# 4
- let bodybg = document.querySelector('body')
- bodybg.style.backgroundColor = 'purple'

# 5 
- let highlightAll = document.querySelectorAll('.highlight')
- for(let i = 0; i < highlightAll.length; i++) {
    highlightAll[i].style.color = 'brown'
}

# 6
- let h1All = document.querySelector('h1')
- h1All.style.fontFamily = 'monospace'

# 7
- let actionIcon = document.querySelectorAll('.action-icon-bg')
- for(let i = 0; i < actionIcon.length; i++) {
    actionIcon[i].style.backgroundColor = 'purple'
}

# 8 
- let formInput = document.querySelectorAll('form > input')
- formInput[0].placeholder = 'identify yourself'

# 9
- let msg = document.querySelector('#message')
- msg.placeholder = 'state your business'

# 10 
- formInput[0].value = 'your nemesis'

# 11
- formInput[1].value = 'koalathebear@gmail.com'

# 12
- formInput[2].value = 'En garde!'

# 13
- formInput[2].disabled = true

# 14
- let bioParent = document.querySelector('.bio-info')
- highlightAll[0].removeChild(bioParent)

# PART 2

# 1.1
- let parentDiv = document.querySelector('section > div')
- let timeTravel = document.querySelectorAll('.bar-default')
- parentDiv.removeChild(timeTravel[2])

# 1.2
- let pikaImg2 = document.querySelector('#right-image > img')
- let dupPika2 = pikaImg2.cloneNode()
- let portfolio = document.querySelector('.portfolio-container')
- portfolio.appendChild(dupPika2)

# 2
- for(let i = 0; i < 10; i++) {
	let pikaDupe = document.createElement('img')
	pikaDupe.src = "images/pikachu-drawing.jpg"
	portfolio.appendChild(pikaDupe)	
}

# 3
- const listItem = document.createElement('li')
- const leftSpan = document.createElement('span')
- let lastUpdated = document.createTextNode('Page last updated on')
- leftSpan.appendChild(lastUpdated)
- listItem.appendChild(leftSpan)
- let bioUl = document.querySelector('.bio-info')
- let rightSpan = document.createElement('span')
- let time = document.createTextNode(new Date())
- rightSpan.appendChild(time)
- listItem.appendChild(rightSpan)
- bioUl.appendChild(listItem)
- listItem.className = 'bio-info-item'
- leftSpan.className = 'bio-info-title'
- rightSpan.className = 'bio-info-value bio-info-time'