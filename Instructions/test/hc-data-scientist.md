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

# You enter the data scientist's office...

You walk to their desk and sit down to talk:

<img src="./media/data-scientist.svg" alt="Hotel" style="width:20%; float:left"> <div class="panel">Hi! I just got hired as the first data scientist and feel a bit like a fish out of water. I don't know if I can help you.</div>

<button class="button" onclick="showContent('id01')">I'm here to help you! Which programming language are you familiar with to train machine learning models?</button>

<button class="button" onclick="showContent('id02')">How are you planning to train the model to predict diabetes in patients?</button>

<div id="id01" class="hidden-content" style="display: none;">
  <div class="selected">I'm here to help you! Which programming language are you familiar with to train machine learning models?</div>
  <div class="panel">I'll be honest with you... I haven't been part of large enterprise data science teams yet. So, I still use Python as that is what I've learned during my studies.</div>
  <button class="response" onclick="window.location.href='../office-health-care';">Thank you! That's great to know. I'll talk to your colleagues to see what works best for this project.</button>
</div>

<div id="id02" class="hidden-content" style="display: none;">
  <div class="selected">How are you planning to train the model to predict diabetes in patients?</div>
  <div class="panel">I'd say it's pretty optimistic of you to think I have a plan. I prefer working in Jupyter notebooks to train machine learning models. I'm not very familiar with any cloud services but could learn to work with another tool I guess...
  </div>
  <button class="response" onclick="window.location.href='../office-health-care';">Thank you! That's great to know. I'll talk to your colleagues to see what works best for this project.</button>
</div>


