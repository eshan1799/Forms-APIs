# Forms-APIs

Generating a celebrations card.

const myForm = document.querySelector('#the-form'); 
myForm.addEventListener("submit", makeCard);

const h1 = document.querySelector('#cardGreeting');
const p = document.querySelector('#type-of-event');
const message = document.querySelector('#cardMessage');

function makeCard(e) { 
    e.preventDefault(); 
    const userGreeting = e.target.greeting.value; 
    const userEvent = e.target.events.value; 
    const userMessage = e.target.message.value; 
    console.log(userGreeting, userEvent, userMessage); 
    h1.textContent = userGreeting; 
    p.textContent= "Have a wonderful " + userEvent; 
    message.textContent= userMessage;

    formDisappear()
};

function formDisappear() {
    myForm.setAttribute("style", "display: none");
}


CSS:
form{
    text-align: center;
}
input{
    margin: 25px auto;

}
h1, h2, p{
    text-align: center;
}
