<style>

.row::after{
  content: "";
  clear: both;
  display: table;
}

.container {
  position: relative;
  width: 40%;
  max-width: 400px;
}

.container img {
  width: 100%;
  height: auto;
}

.container .btn {
  position: absolute;
  top: 30%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: white;
  color: black;
  font-size: 14px;
  padding: 12px px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

.container .btn:hover {
  background-color: black;
  color: white;
}
</style>

## You're in the office of Proseware

Choose who you want to talk to next. Finally, when you gathered all information, you should talk to the project manager.

<div class="row">
  <div class="container">
    <img src="./media/door.svg" alt="Talk to the data scientist" style="width:100%">
      <button class="btn" onclick="window.location.href='../hc-data-scientist';">Talk to the data scientist</button>
    </div>
    <div class="container">
    <img src="./media/door.svg" alt="Talk to the software engineer" style="width:100%">
      <button class="btn" onclick="window.location.href='../hc-software-engineer';">Talk to the software engineer</button>
    </div>

<div class="row">
  <div class="container">
    <img src="./media/door.svg" alt="Talk to the business user" style="width:100%">
      <button class="btn" onclick="window.location.href='../hc-business-user';">Talk to the business users</button>
    </div>
    <div class="container">
    <img src="./media/door.svg" alt="Talk to the data engineer" style="width:100%">
      <button class="btn" onclick="window.location.href='../hc-data-engineer';">Talk to the data engineer</button>
    </div>
  </div>

<div class="row">
  <div class="container">
    <img src="./media/door-health-care.svg" alt="Talk to the project manager" style="width:100%">
      <button class="btn" onclick="window.location.href='../hc-end';">Talk to the project manager</button>
  </div>