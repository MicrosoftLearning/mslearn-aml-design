<style>
.button  {
  border: none;
  color: black;
  width: 75%;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #70AD47;
  border-radius:30px 5px 30px 30px ;
  transition-duration: 0.4s;
  text-align: right;
  float: right;
}
.button:hover  {
  background-color: #70AD47;
  color: white; 
  border: 2px solid #70AD47;
}
.answers .button2  {
  border: 2px solid white;
  color: white;
  width: 25%;
  height: 50px;
  background-color: #008CBA;
  transition-duration: 0.4s;
  float: left;
  clear: right;
}
.answers .button2:hover  {
  background-color: white;
  color: black; 
  border: 2px solid #008CBA;
}
.panel {
  background-color: white;
  border: 2px solid #787878;
  color: black;
  border-radius: 5px 30px 30px 30px;
  padding: 20px 20px;
  width: 75%;
  float: left;
  margin-top: 20px;
  margin-bottom: 20px;
  text-align: left;
}
.header {
  background-color: white;
  border: 2px solid #008CBA;
  color: black;
  padding: 12px 28px;
  width: 75%;
  margin-top: 20px;
  text-align: left;
  clear: right;
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

<img style="float: right; width:5%; display:box; clear: right; margin-top: 10px;" src="./media/help.png">

# You enter the data scientist's office...

You meet with the data scientist. He starts the conversation:

<div class= "panel">Hi! I'm Albert, the resident data scientist. I've been working here for some years already so feel free to ask me anything you need to know about how we trained the model.
</div>

<button class="button" onclick="document.getElementById('id01').style.display='block'">Where is the data currently stored?</button>

<button class="button" onclick="document.getElementById('id02').style.display='block'">Can I get a preview of the data?</button>

<button class="button" onclick="document.getElementById('id03').style.display='block'">Which language do you use?</button>

<div id="id01" style="display:none;">
<div class= "panel">The data is stored in a patient database.</p>
</div>
<button class="resetbutton" onclick="window.location.href='../start-01-data';">Reset game and go back to start</button>
</div>

<div id="id02" style="display:none;">
<div class= "panel">If we open the file, the first few rows of data like this:
<code>
PatientID,Pregnancies,PlasmaGlucose,DiastolicBloodPressure,TricepsThickness,SerumInsulin,BMI,DiabetesPedigree,Age,Diabetic
1354778,0,171,80,34,23,43.50972593,1.213191354,21,0
1147438,8,92,93,47,36,21.24057571,0.158364981,23,0
1640031,7,115,47,52,35,41.51152348,0.079018568,23,0
1883350,9,103,78,25,304,29.58219193,1.282869847,43,1
</code></p>
</div>
<button class="resetbutton" onclick="window.location.href='../start-01-data';">Reset game and go back to start</button>
</div>

<div id="id03" style="display:none;">
<div class= "panel">I'm mostly comfortable with Python, so that's also what we all tend to use.
</div>
<button class="resetbutton" onclick="window.location.href='../start-01-data';">Reset game and go back to start</button>
</div>




