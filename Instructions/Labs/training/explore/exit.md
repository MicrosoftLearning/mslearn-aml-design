<style>
.button  {
  border: none;
  color: black;
  width: 100%;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #008CBA;
  transition-duration: 0.4s;
}
.button:hover  {
  background-color: #008CBA;
  color: white; 
  border: 2px solid #008CBA;
}
.resetbutton  {
  border: none;
  color: black;
  float: right;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #f44336;
  transition-duration: 0.4s;
}
.resetbutton:hover  {
  background-color: #f44336;
  color: white; 
  border: 2px solid #f44336;
}
</style>

## You've heard enough?

Great! Now that you have enough information, you can help us by giving advice on what to do. There are three scenarios we want to implement in the near future.

## Which scenario would you like to hear about?

<button class="button" onclick="window.location.href='../advice/01';">Give advice on how to detect diabetes.</button>

<button class="button" onclick="window.location.href='../advice/02';">Give advice on how to detect skin abnormalities.</button>

<button class="button" onclick="window.location.href='../advice/03';">Give advice on how to analyze patient satisfaction.</button>

<p style="text-align:right;"><i>All progress will be lost when you reset the game.</i></p>

<button class="resetbutton" onclick="window.location.href='../../00-start-training';">Reset game and go back to start</button>
