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

## Design a machine learning model training solution

Welcome to Proseware! Proseware is a start-up which specializes in creating solutions for health care. 

Currently, we're working on several solutions which will support health care practitioners like doctors and nurses in their day-to-day job. By helping them be more data-driven, we're hoping to help them faster diagnose diseases and minimize risk.

We hired you to be our lead data scientist. We want you to help us create machine learning models which will support the solutions we're developing.

### Get more information
Need to know more before you can give advice? Select a question below to find out more about the use case.

<p id="hints"></p>

<script>
let hintUsed = 0;
</script>

<details>
<summary><font size="+1">What can you tell me about the current data science team?</font></summary>
<script>
if (hintUsed = 0) {
  answer = "It's a small team, we only have two other data scientists you'll be leading. We therefore advise you to allocate your time wisely. Ideally, we want our data scientists to collaborate and work on each others' work. How great would it be if we would have some kind of library of code snippets you could reuse for new projects to speed up the development process?"; 
} else {
  answer = "You already used one hint.";
}
document.getElementById("hints").innerHTML = answer;
</script>
</details>

<details>
<summary><font size="+1">Which programming language do the data scientists use?</font></summary>
<script>
if (hintUsed = 0) {
  answer = "The data scientists only work in Python. They work in Jupyter notebooks.";
} else {
  answer = "You already used one hint.";
}
document.getElementById("hints").innerHTML = answer;
</details>



## Which tool would you recommend we use to train the model?

<button class="button" onclick="window.location.href='04B';">Azure Databricks</button>

<button class="button" onclick="window.location.href='04A';">Azure Machine Learning</button>

<button class="button" onclick="window.location.href='04B';">Azure Synapse Analytics</button>

<button class="button" onclick="window.location.href='04B';">Azure Data Science Virtual Machine</button>

<p style="text-align:right;"><i>All progress will be lost when you reset the game.</i></p>

<button class="resetbutton" onclick="window.location.href='../../00-start-training';">Reset game and go back to start</button>


<br>
<details>
<summary><font size="+1">What tools do you currently use for machine learning projects?</font></summary>

The data science team is brand new so we haven't created any guidelines on what the data scientists should use yet. That's where we need you! 

So far, the data scientists seem to be working on their own devices. Which is fine for now, but not scalable. We want them to work in Azure so that we can use more scalable and cost-efficient compute.
</details>

<br>
<details>
<summary><font size="+1">Which programming language do the data scientists use?</font></summary>

The data scientists only work in Python. They work in Jupyter notebooks.
</details>

<br>
<details>
<summary><font size="+1">Do you already use the cloud for other data-related projects?</font></summary>

We work with Azure for some other data-related projects. Currently, we mostly focus on getting insights from operational data. We ingest and transform data with Azure Synapse Analytics. The transformed data is stored in an Azure SQL Database which serves a Power BI report. 
</details>