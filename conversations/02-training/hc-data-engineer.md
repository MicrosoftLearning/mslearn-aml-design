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
.selected  {
  border: none;
  color: black;
  width: 75%;
  padding: 12px 28px;
  background-color: white;
  border: 2px solid #70AD47;
  border-radius:30px 5px 30px 30px ;
  text-align: right;
  float: right;
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
.response  {
  border: none;
  color: black;
  float: right;
  padding: 12px 28px;
  background-color: white;
  border-radius:30px 5px 30px 30px ;
  border: 2px solid #70AD47;
  transition-duration: 0.4s;
}
.response:hover  {
  background-color: #70AD47;
  color: white; 
  border: 2px solid #70AD47;
}
</style>

<script>
function showContent(id) {
  // Hide all hidden content
  var elements = document.getElementsByClassName('hidden-content');
  for (var i = 0; i < elements.length; i++) {
    elements[i].style.display = 'none';
  }

  // Show the selected hidden content
  var selectedElement = document.getElementById(id);
  if (selectedElement) {
    selectedElement.style.display = 'block';
  }

  // Remove unselected buttons
  var buttons = Array.from(document.getElementsByClassName('button'));
  buttons.forEach(function(button) {
    if (button.id !== id) {
      button.remove();
    }
  });
}
</script>

<img style="float: right; width:5%; display:box; clear: right; margin-top: 10px;" src="./media/help.png">

# You enter the data engineer's office...

You walk to their desk and sit down to talk:

<img src="./media/data-engineer.svg" alt="Hotel" style="width:20%; float:left"> 

<div class="panel">Oh hello. I guess you're doing something with data science right? I'm not too familiar with that whole thing, but I guess I could help with some questions around our data estate.</div>

<button class="button" onclick="showContent('id01')">Don't worry about the data science. Which cloud services do you already use for other data projects?</button>

<button class="button" onclick="showContent('id02')">The data scientists will need historical data that includes a patient's medical information and whether they have diabetes. Do you know where that data is currently stored?</button>

<div id="id01" class="hidden-content" style="display: none;">
  <div class="selected">Don't worry about the data science. Which cloud services do you already use for other data projects?</div>
  <div class="panel">For our main data analysis, we load data into a data lake and transform it with Azure Data Factory. The clean data is stored in a SQL database to serve a Power BI report.</div>
  <button class="response" onclick="window.location.href='./hc-office';">Thank you for taking the time to answer my question! I'll leave you to it.</button>
</div>

<div id="id02" class="hidden-content" style="display: none;">
  <div class="selected">The data scientists will need historical data that includes a patient's medical information and whether they have diabetes. Do you know where that data is currently stored?</div>
  <div class="panel">In line with government regulations, we use software that medical professionals use to enter and retrieve patient information. Whenever we want to use data from the software, we pull anonymized data through an API. We're not allowed to do any data analysis directly in the software.
  </div>
  <button class="response" onclick="window.location.href='./hc-office';">Thank you for taking the time to answer my question! I'll leave you to it.</button>
</div>


