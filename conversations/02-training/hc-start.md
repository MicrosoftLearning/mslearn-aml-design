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

<img src="./media/welcome-project-manager.svg" alt="Hotel" style="width:20%; float:left"> <div class="panel">Welcome to Proseware! We’re a start-up focused on revolutionizing healthcare through innovative applications. I'm Taylor and I work here as a project manager.</div>

<button class="button" onclick="showContent('id01')">That sounds fascinating! How does this application work?</button>

<button class="button" onclick="showContent('id02')">That’s really interesting! I’d like to learn more about the technical aspects. Could you suggest someone I can talk to about the data science behind the application?</button>

<div id="id01" class="hidden-content" style="display: none;">
  <div class="selected">That sounds fascinating! How does this application work?</div>
  <div class="panel">Great question! Our application utilizes machine learning algorithms to analyze various medical parameters, such as BMI and age, to predict the likelihood of a patient having diabetes. Medical professionals can enter a patient’s information into the app and use the prediction to decide on further actions.</div>
  <button class="response" onclick="showContent('id03')">That’s really interesting! I’d like to learn more about the technical aspects. Could you suggest someone I can talk to about the data science behind the application?</button>
</div>

<div id="id02" class="hidden-content" style="display: none;">
  <div class="selected">That’s really interesting! I’d like to learn more about the technical aspects. Could you suggest someone I can talk to about the data science behind the application?</div>
  <div class="panel">Certainly! Feel free to explore our office and chat with our team members. Once you’ve gathered the information you need, come back to me and let’s discuss the best solution for this project.
  </div>
  <button class="response" onclick="window.location.href='./hc-office';">Thank you for the information. I'm excited to explore the office and speak with the team.</button>
</div>

<div id="id03" class="hidden-content" style="display: none;">
  <div class="selected">That sounds fascinating! How does this application work?</div>
  <div class="panel">Great question! Our application utilizes machine learning algorithms to analyze various medical parameters, such as BMI and age, to predict the likelihood of a patient having diabetes. Medical professionals can enter a patient’s information into the app and use the prediction to decide on further actions.</div>
  <div class="selected">That’s really interesting! Could you suggest someone I can talk to about the data science behind the application?</div>
  <div class="panel">Certainly! Feel free to explore our office and chat with our team members. Once you’ve gathered the information you need, come back to me and let’s discuss the best solution for this project.</div>
  <button class="response" onclick="window.location.href='./hc-office';">Thank you for the information. I'm excited to explore the office and speak with the team.</button>
</div>

