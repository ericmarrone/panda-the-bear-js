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

4. 
