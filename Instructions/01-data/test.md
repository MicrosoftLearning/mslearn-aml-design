<style>
.button  {
  border: none;
  color: black;
  width: 75%;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #70AD47;
  border-radius:30px 30px 30px 5px;
  transition-duration: 0.4s;
  text-align: left;
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
  border-radius:30px 30px 5px 30px;
  padding: 20px 20px;
  width: 75%;
  float: right;
  margin-top: 20px;
  margin-bottom: 20px;
  text-align: right;
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
</style>

<img style="float: right; width:30%; display:box; clear: right; margin-top: 10px;" src="./media/0-points.png">

# Question 1/5

You meet with the data lead. He starts the conversation:

<div class= "panel">We have already collected data that correlates with diabetes, such as the number of pregnancies, age and BMI.
</div>

<button class="button" onclick="document.getElementById('id01').style.display='block'">Ask: Where is the data currently stored?</button>

<div id="id01" class="panel" style="display:none;">
  <p>The data is stored in a patient database.</p>
</div>

<button class="button" onclick="document.getElementById('id02').style.display='block'">Ask: Can I get a preview of the data?</button>

<div id="id02" class="panel" style="display:none;">
  <p>If we open the file, the first few rows of data like this:
<code>
PatientID,Pregnancies,PlasmaGlucose,DiastolicBloodPressure,TricepsThickness,SerumInsulin,BMI,DiabetesPedigree,Age,Diabetic
1354778,0,171,80,34,23,43.50972593,1.213191354,21,0
1147438,8,92,93,47,36,21.24057571,0.158364981,23,0
1640031,7,115,47,52,35,41.51152348,0.079018568,23,0
1883350,9,103,78,25,304,29.58219193,1.282869847,43,1
</code></p>
</div>

<button class="button" onclick="document.getElementById('id03').style.display='block'">Say: I think I have all the information I need. What advice do you need?</button>

<div id="id03" style="display:none;">
<div class= "panel">What kind of data do we have?
</div>

<div class="header">Answer by selecting one of the following options:</div>
<div class = "answers">
  <button class="button2" onclick="window.location.href='02A';">Structured</button>
  <button class="button2" onclick="window.location.href='02B';">Semi-structured</button>
  <button class="button2" onclick="window.location.href='02B';">Unstructured</button>
</div>
</div>




