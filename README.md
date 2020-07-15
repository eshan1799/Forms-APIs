# Forms-APIs

Generating a celebrations card.

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Celebration Card</title>
    <script defer src="/Users/rebeccatabbener/Documents/Development/greetingCard/action.js"></script>
</head>
<body>
    <form id="the-form" >
        <label for="greeting">Greeting:</label>
        <input id="greeting" type="text" placeholder="Greeting">
        <br>
        <label for="events">Type of event:</label>
        <select id="events" name="cars">
            <option value="New Year">New Year</option>
            <option value="Christmas">Christmas</option>
            <option value="Easter">Easter</option>
          </select>
        <br>
        <label for="message">Message:</label>
        <input id="message" type="text" placeholder="Message">
        <br>
        <input id= "submit" type="submit" value="send">
    </form>
    <section>
        <h1 id="cardGreeting"></h1>
        <p id="type-of-event"> </p>
        <p id="cardMessage"></p>
    </section>
</body>
</html>
