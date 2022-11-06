<style>
.button  {
  color: white;
  width: 100%;
  padding: 8px 28px;
  background-color: #70AD47;
  transition-duration: 0.4s;
  text-align: left;
  border: 2px solid #70AD47;
}
.button:hover  {
  background-color: #507E32;
  color: white; 
  border: 2px solid #507E32;
}
.answerbutton  {
  border: none;
  color: black;
  width: 100%;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #008CBA;
  transition-duration: 0.4s;
}
.answerbutton:hover  {
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

<img style="float: right;width:30%;" src="./media/0-points.png">

### Question 1/5

# What type of data do we currently have?

We have already collected data that correlates with diabetes, such as the number of pregnancies, age and BMI.

<button class="button" onclick="document.getElementById('id01').style.display='block'">Ask: Where is the data currently stored?</button>

<div id="id01" style="display:none;">
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

## Select your answer:

<button class="answerbutton" onclick="window.location.href='02A';">Structured</button>

<button class="answerbutton" onclick="window.location.href='02B';">Semi-structured</button>

<button class="answerbutton" onclick="window.location.href='02B';">Unstructured</button>

<p style="text-align:right;"><i>All progress will be lost when you reset the game.</i></p>

<button class="resetbutton" onclick="window.location.href='../start-01-data';">Reset game and go back to start</button>


