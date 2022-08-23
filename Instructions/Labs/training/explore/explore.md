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

As a data scientist, we expect you to help us create machine learning models which will support the solutions we're developing.

### Select a question to view the answer

<br/>
<details>
<summary><font size="+1">Could you tell me more about the team I'll work with?</font></summary>

We only just decided to work with machine learning models, so the current data science team is quite small. We therefore advise you to allocate your time wisely. 

It would be really helpful if you could work more closely together with the other two data scientists. You should be able to build on each other's work and easily share your code. Preferably, we would want to have a library of code snippets you could reuse for new projects to speed up the development process.
</details>

<br/>
<details>
<summary><font size="+1">What tools do you currently use for machine learning projects?</font></summary>

We just started our data science team. So far, the data scientists seem to be working on their own devices. We haven't explored other options yet for them to work in the Azure cloud. 

Ideally, we do want them to work with a cloud service so that we can use more scalable and cost-efficient compute. Since we work a lot with medical and privacy-sensitive data, we also want to avoid people having a copy of the data on their own device.
</details>

<br/>
<details>
<summary><font size="+1">Which programming language do these data scientists use?</font></summary>

The data scientists only work in Python. They work in Jupyter notebooks.
</details>

<br/>
<details>
<summary><font size="+1">Do you already use the cloud for other data-related projects?</font></summary>

Our data engineers and data analysts are already working with Azure. One of the first large data-related projects we implemented was to create a data ingestion and transformation pipeline. The data engineers have mostly worked with Azure Synapse Analytics to create those pipelines.

Data is collected from multiple sources, like the Customer Relationship Management (CRM) system we use for patient data. After collection, the data is cleaned, prepped, and saved to a SQL database. 

Finally, data analysts use Power BI on top of that SQL database to visualize necessary insights. They've created reports which are used by our customers on a daily basis.
</details>

## Which tool would you recommend we use to train the model?

<button class="button" onclick="window.location.href='04B';">Azure Databricks</button>

<button class="button" onclick="window.location.href='04A';">Azure Machine Learning</button>

<button class="button" onclick="window.location.href='04B';">Azure Synapse Analytics</button>

<button class="button" onclick="window.location.href='04B';">Azure Data Science Virtual Machine</button>

<p style="text-align:right;"><i>All progress will be lost when you reset the game.</i></p>

<button class="resetbutton" onclick="window.location.href='../../00-start-training';">Reset game and go back to start</button>
