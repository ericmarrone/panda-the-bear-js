## Answers

var body = document.body;

1. var profileImage = body.querySelector('.profile-image');
  profileImage.src = "https://placebear.com/400/400";

1. var leftImage = body.querySelector('#left-image > img');
leftImage.src = "https://placebear.com/325/225";

2. var heading = body.querySelector('section').querySelector('.highlight');
  heading.innerText = "Eric";

3. var employment = body.querySelector('#employment > h3');
  var newHTML = employment.innerHTML.replace("Employment", "Test");
  employment.innerHTML = newHTML

4. body.style.backgroundColor = "blue";

5. var highlights = body.querySelectorAll(".highlight");
for(i=0;i<highlights.length;i++){highlights[i].style.color = 'red'};

6. var title = body.querySelector('h1')
title.style.fontFamily = 'monospace';

7. var roundIcons = body.querySelectorAll('.action-icon-container > a');

  roundIcons.forEach(function(icon) {
      icon.style.backgroundColor = "red";
  });

8. var formName = body.querySelector('#name');
  formName.placeholder = "Identify yourself";

9. var formMessage = body.querySelector('#message');
formMessage.placeholder = "state your business";

10. formName.value = "your nemisis";
"your nemisis"

11. var formEmail = body.querySelector('#email');

formEmail.value = "koalathebear@gmail.com";

12. var formSubmit = body.querySelector('#submit');
formSubmit.value = "En garde!";

13. formSubmit.disabled = true
14. var personalInfo = body.querySelectorAll('.bio-info-value');
personalInfo.forEach(function(item) {
    item.innerText = "";
});
