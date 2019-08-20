Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

1.  document.querySelector('#left-image, img').src="https://2.bp.blogspot.com/-j4yOugUEOpU/T7rQz6s0PFI/AAAAAAAAB7g/0EPYcsMq660/s320/Kathmandu01.JPG"

document.querySelector('#left-image, img').src="https://placebear.com/400/400"
"https://placebear.com/400/400"


Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

document.querySelector('#left-image.portfolio-image img').src="https://placebear.com/325/225"


2. Select the heading that says "Panda the Bear" and change it to your own name.

document.querySelector('h1.highlight').innerHTML="Mark Jarvis"

3. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

document.querySelector('h3.info-title').innerHTML="Skools"

Change the colour of the body.

document.querySelector('body').style.backgroundColor="blue"

Change the colour of each element using the highlight class. Use a for loop to do this.
for (i = 0;i < hightlights.length; i++){hightlights[i].style.backgroundColor="purple"}

Change the font family of the h1 to 'monospace'.

document.querySelector('h1').style.fontFamily="monospace"

Find a way to select the round icons in the sidebar and then change their colour.

let icons = document.querySelectorAll('.action-icon-bg')
for (i=0; i < icons.length; i++){icons[i].style.backgroundColor="blue"}

Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

document.querySelector('.contact-info').placeholder="identify yourself"

Change the placeholder attribute of the message field to "state your business".

document.querySelector('#message').placeholder="state your business"

Give the name field a "value" attribute of "your nemesis".

document.querySelector('#name').value="your nemesis"

Change the value attribute of the email field to "koalathebear@gmail.com".

document.querySelector('#email').value="koalathebear@gmail.com"

Change the value of the submit button on the contact form to "En garde!".

document.querySelector('#submit').value="En garde!"

We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

document.querySelector('#submit').disabled=true
true

We should help Panda protect their privacy by erasing their personal details from the sidebar.

items = document.querySelectorAll('.bio-info .bio-info-value')
for (i = 0; i < items.length;i++){items[i].innerText=''}

remove a node 

stuff = document.querySelector('.bar-default #time-travel')
stuff.remove()

Cloning a node and placing it at the end of a section also doing so multiple times

section = document.querySelector('section > :nth-child(2)')
section.appendChild(pikaClone)
for (i = 0; i < 10; i++){section.appendChild(pikachuPic.cloneNode(true))}

adding another element

let bioList = document.querySelector('.bio-list') bioList.appendChild(listItem) let today = new Date() let rightSpan = document.createElement('span') rightSpan.innerText = today bioList.lastElementChild.appendChild(rightSpan) bioList.lastElementChild.classList.add('bio-info-item') bioList.lastElementChild.firstElementChild.classList.add('bio-info-title') bioList.lastElementChild.lastElementChild.classList.add('bio-info-published-date')