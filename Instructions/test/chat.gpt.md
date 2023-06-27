<style>
  .grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 20px;
  }

  .door {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #eaeaea;
    padding: 20px;
    border-radius: 10px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  .door:hover {
    background-color: #d5d5d5;
  }

  .door img {
    max-width: 100%;
    max-height: 100%;
  }
</style>

<div class="grid">
  <div class="door" onclick="handleDoorClick(1)">
    <img src="./media/door.svg" alt="Door 1">
  </div>
  <div class="door" onclick="handleDoorClick(2)">
    <img src="./media/door.svg" alt="Door 2">
  </div>
  <div class="door" onclick="handleDoorClick(3)">
    <img src="./media/door.svg" alt="Door 3">
  </div>
  <div class="door" onclick="handleDoorClick(4)">
    <img src="./media/door.svg" alt="Door 4">
  </div>
  <div class="door" onclick="handleDoorClick(5)">
    <img src="./media/door.svg" alt="Door 5">
  </div>
</div>

<script>
  function handleDoorClick(doorNumber) {
    // Handle the click event for the respective door
    console.log("Door", doorNumber, "clicked!");
  }
</script>
