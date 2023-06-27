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

# You enter the building...

You are greeted at the door:

<img src="./media/welcome-project-manager.svg" alt="Hotel" style="width:20%; float:left"> <div class="panel">Hi again! Do you have all the information you need to help me?</div>

<button class="button" onclick="showContent('id01')">Yes! I talked to enough of your colleagues to help you and give advice on which solution best suits your needs.</button>

<button class="button" onclick="window.location.href='../office-health-care';">I could use some more time with your colleagues. Let me go back to talk to them.</button>

<div id="id01" class="hidden-content" style="display: none;">
  <div class="selected">Yes! I talked to enough of your colleagues to help you and give advice on which solution best suits your needs.</div>
  <div class="panel">Perfect! What do you want to focus on?</div>
  <button class="response" onclick="showContent('id01-01')">A - long answer to make sure it's below the response</button>
  <button class="response" onclick="showContent('id01-02')">B - long answer to make sure it's below the response</button>
  <button class="response" onclick="showContent('id01-03')">C - long answer to make sure it's below the response</button>
  <button class="response" onclick="showContent('id01-04')">D - long answer to make sure it's below the response </button>
</div>

<div id="id01-02" class="hidden-content" style="display: none;">
  <div class="selected">A - long answer to make sure it's below the response</div>
  <div class="panel">Certainly! Feel free to explore our office and chat with our team members. Once you’ve gathered the information you need, come back to me and let’s discuss the best solution for this project.
  </div>
  <button class="response" onclick="window.location.href='../start-01-data';">Thank you for the information. I'm excited to explore the office and speak with the team.</button>
</div>

<div id="id03" class="hidden-content" style="display: none;">
  <div class="selected">That sounds fascinating! How does this application work?</div>
  <div class="panel">Great question! Our application utilizes machine learning algorithms to analyze various medical parameters, such as BMI and age, to predict the likelihood of an individual having diabetes. Medical professionals can enter a patient’s information into the app and use the prediction to decide on further actions.</div>
  <div class="selected">That’s really interesting! Could you suggest someone I can talk to about the data science behind the application?</div>
  <div class="panel">Certainly! Feel free to explore our office and chat with our team members. Once you’ve gathered the information you need, come back to me and let’s discuss the best solution for this project.</div>
  <button class="response" onclick="window.location.href='../start-01-data';">Thank you for the information. I'm excited to explore the office and speak with the team.</button>
</div>

