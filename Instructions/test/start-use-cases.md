<style>
.row::after{
    content: "";
    clear: both;
    display: table;
}

.container {
  float: left;
  width: 33.3%;
}

.container img {
  width: 100%;
  height: auto;
}

.container .btn {
  position: absolute;
  top: 110%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: black;
  color: white;
  font-size: 16px;
  padding: 16px 30px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

.container .btn:hover {
  background-color: white;
  color: black;
}
</style>

# Start

Welcome to this game. Choose your adventure by selecting one of the options below.

<div class="row">
  <div class="container">
    <img src="./media/hotel-icon.jpg" alt="Hotel" style="width:100%">
    <button class="btn">Hotel</button>
  </div>
  <div class="container">
    <img src="./media/supermarket-icon.jpg" alt="Supermarket" style="width:100%">
    <button class="btn">Supermarket</button>
  </div>
  <div class="container">
    <img src="./media/hospital-icon.jpg" alt="Health care" style="width:100%">
    <button class="btn">Health care</button>
  </div>
</div>

