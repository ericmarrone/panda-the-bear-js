# Answers

# Part 1

`var body = document.body;`

### 1
```
var profileImage = body.querySelector('.profile-image');
profileImage.src = "https://placebear.com/400/400";
```

### 2
```
var leftImage = body.querySelector('#left-image > img');
leftImage.src = "https://placebear.com/325/225";
```

### 3
```
var heading = body.querySelector('section').querySelector('.highlight');
heading.innerText = "Eric";
```

### 4
```
var employment = body.querySelector('#employment > h3');
var newHTML = employment.innerHTML.replace("Employment", "Test");
employment.innerHTML = newHTML
```

### 5
`body.style.backgroundColor = "blue";`

### 6
```
var highlights = body.querySelectorAll(".highlight");
for(i=0;i<highlights.length;i++){highlights[i].style.color = 'red'};
```

### 7
```
var title = body.querySelector('h1')
title.style.fontFamily = 'monospace';
```

### 8
```
var roundIcons = body.querySelectorAll('.action-icon-container > a');

roundIcons.forEach(function(icon) {
  icon.style.backgroundColor = "red";
});

```

### 9
```
var formName = body.querySelector('#name');
  formName.placeholder = "Identify yourself";
```

### 10
```
var formMessage = body.querySelector('#message');
formMessage.placeholder = "state your business";
```

### 11
`formName.value = "your nemisis";`

### 12
```
var formEmail = body.querySelector('#email');

formEmail.value = "koalathebear@gmail.com";
```

### 13
```
var formSubmit = body.querySelector('#submit');
formSubmit.value = "En garde!";
```

### 14
`formSubmit.disabled = true`

### 15
```
var personalInfo = body.querySelectorAll('.bio-info-value');
personalInfo.forEach(function(item) {
item.innerText = "";
});
```

# Part 2

## Removing Elements
### 1

```
$("#time-travel").parent().remove();
```

## Adding Elements
### 1

```
var pikachu = body.querySelector('#right-image > img');
var dupPikachu = pikachu.cloneNode();
var element = document.querySelector('.portfolio-container');
element.appendChild(dupPikachu);
```

### 2

```
for (var i = 0; i <= 10; i++) {
    element.appendChild(dupPikachu.cloneNode());
};
```

### 3

```
var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
var rightSpan = document.createElement('span');
var dateText = document.createTextNode(new Date());
rightSpan.appendChild(dateText);
listItem.appendChild(rightSpan);
var bioInfo = body.querySelector('.bio-info');
bioInfo.appendChild(listItem);
listItem.className = "bio-info-item";
rightSpan.className = "bio-info-title";
rightSpan.classList.add("bio-info-value", "bio-info-date");
```
