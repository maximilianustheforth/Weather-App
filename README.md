# Weather-App
weather application style page made by html&amp;css
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Weathe App</title>
    <style>
      h1 {
        display: block;
        text-align: center;
        font-size: 18px;
        font-family: Arial, Helvetica, sans-serif;
      }
      h1:hover {
        color: rgb(61, 200, 243);
      }
      h2,
      h3,
      h4 {
        max-width: 400px;
        margin: 0 auto;
      }
      h2 {
        color: rgb(52, 100, 190);
        background: #fff;
        font-size: 18px;
        text-align: center;
        padding: 50px, 25px;
        border: 25 rgb(255, 255, 255);
        border-radius: 4px;
        font-family: Arial, Helvetica, sans-serif;
      }
      h2:hover {
        background-color: rgb(244, 245, 248);
        color: rgb(61, 200, 243);
        transition: all, 1s, ease-in-out;
        cursor: pointer;
      }
      h3 {
        background-color: #fff;
        color: rgb(52, 100, 190);
        font-size: 18px;
        text-align: center;
        padding: 50px, 25px;
        border: 25 rgb(255, 255, 255);
        border-radius: 4px;
        font-family: Arial, Helvetica, sans-serif;
      }
      h3:hover {
        background-color: rgb(244, 245, 248);
        color: rgb(61, 200, 243);
        transition: all, 1s, ease-in-out;
        cursor: pointer;
      }

      h4 {
        background-color: #fff;
        color: rgb(52, 100, 190);
        font-size: 18px;
        text-align: center;
        padding: 50px, 25px;
        border: 25 rgb(255, 255, 255);
        border-radius: 4px;
        font-family: Arial, Helvetica, sans-serif;
      }
      h4:hover {
        background-color: rgb(244, 245, 248);
        color: rgb(61, 200, 243);
        transition: all, 1s, ease-in-out;
        cursor: pointer;
      }
      p {
        display: block;
        font-size: 20px;
        text-align: center;
        color: black;
      }
      .wtwo {
        color: rgb(39, 96, 172);
        font-size: 34px;
        line-height: 45px;
        text-align: center;
        display: block;
        text-decoration: overline;
        border: 1px;
        transition: all 200ms;
      }
      .wtwo:hover {
        color: rgb(61, 200, 243);
      }
      .wthree {
        text-align: center;
        font-size: 18px;
        display: block;
        margin-top: 10px;
        font-weight: lighter;
        opacity: 70%;
      }
      .wthree:hover {
        color: rgb(61, 200, 243);
      }
      .wone {
        color: rgb(39, 96, 172);
        text-align: center;
        font-size: 22px;
        display: block;
        margin: 50 auto 0;
        padding: 50, -10px;
        border: 10px, normal, rgb(39, 96, 172);
        border-radius: 4px;
        transition: all, 200ms, ease-in-out;
      }
      .wfour {
        text-align: center;
        font-size: 18px;
        font-weight: lighter;
        opacity: 70%;
      }
      .wfive {
        color: rgb(39, 96, 172);
        text-align: center;
        font-size: 22px;
        display: block;
        margin: 50 auto 0;
        padding: 50, -10;
        border: 10px, normal, rgb(39, 96, 172);
        border-radius: 4px;
        transition: all, 200ms, ease-in-out;
      }
      .wsix {
        text-align: center;
        font-size: 18px;
        font-weight: lighter;
        opacity: 70%;
      }
      .wseven {
        color: rgb(39, 96, 172);
        text-align: center;
        font-size: 22px;
        display: block;
        margin: 50 auto 0;
        padding: 50, -10;
        border: 10px, normal, rgb(39, 96, 172);
        border-radius: 4px;
        transition: all, 200ms ease-in-out;
      }

      .weight {
        text-align: center;
        font-size: 18px;
        font-weight: lighter;
      }
      button {
        background-color: rgb(39, 96, 172);
        color: #fff;
        display: block;
        margin: 0 auto;
        padding: 25px;
        border: 15px none #fff;
        border-radius: 50px;
        font-size: 22px;
        position: right;
      }
      button:hover {
        color: rgb(39, 96, 172);
        background-color: #fff;
        cursor: pointer;
        transition: all 200ms ease-in-out;
      }
      .coder-info {
        display: block;
        text-align: center;
        margin: 15px;
        opacity: 70%;
        font-family: "Times New Roman", Times, serif;
      }
      .line {
        display: inline;
      }
      .weight {
        font-weight: lighter;
        opacity: 70%;
      }
      .wnine {
        font-weight: bold;
        opacity: 100%;
      }
    </style>
  </head>
  <body>
    <h1>
      <p class="emoji">🌦️</p>
      <strong class="wtwo"> Currently 34° in Tehran </strong>
      <span class="wthree">18° /<span class="wnine"> 36°</span></span>
    </h1>
    <h2>
      <p class="wone">🌥️Tomorrow</p>
      <span class="wfour">17° /</span>
      38°
    </h2>
    <h3>
      <p class="wfive">☀️Thursday</p>
      <span class="wsix">19° /</span> 39°
    </h3>
    <h4>
      <p class="wseven">🌤️Wednesday</p>
      <span class="weight">16°/ </span>32°
    </h4>
    <br />
    <button>change city</button>
    <span class="coder-info"> coded by melika ziarati </span>
    <script>
      function contactUs() {
        let city = prompt("Which city do you live in?");
        let temperature = prompt(
          "What is the current temperature in your city"
        );
        let currentTemperature = document.querySelector(".wtwo");
        let emojiStyle = document.querySelector(".emoji");
        if (temperature < 0) {
          currentTemperature.innerHTML =
            "Currently " + temperature + "° " + "in " + city;
          emojiStyle.innerHTML = "😰";
        } else {
          currentTemperature.innerHTML =
            "Currently " + temperature + "° " + "in " + city;
          emojiStyle.innerHTML = "😃";
        }
      }
      let button = document.querySelector("button");
      button.addEventListener("click", contactUs);
    </script>
  </body>
</html>
