<template>
  <div id="app">
    <div class="naslov-strani">
      <h1>
        Razvrsti stvari
      </h1>
    </div>
    <main class="flexbox">

      <Board id="board-1">
        <div class="ime-stolpca-1">
          <h3>
            ZNAMKE AVTOV
          </h3>
        </div>
        <br/>
        <Card id="card-1" draggable="true">
          <p>BMW</p>
        </Card>

        <Card id="card-2" draggable="true">
          <p>AUDI</p>
        </Card>

        <Card id="card-3" draggable="true">
          <p>TROBENTICA</p>
        </Card>

        <Card id="card-4" draggable="true">
          <p>HONDA</p>
        </Card>

        <Card id="card-5" draggable="true">
          <p>DACIA</p>
        </Card>

      </Board>

      <Board id="board-2">
       <div class="ime-stolpca-1">
          <h3>
            ROŽE
          </h3>
        </div>
      <br/>
        <Card id="card-6" draggable="true">
          <p>ORHIDEJA</p>
        </Card>

        <Card id="card-7" draggable="true">
          <p>NAGELN</p>
        </Card>

        <Card id="card-8" draggable="true">
          <p>RENAULT</p>
        </Card>

        <Card id="card-9" draggable="true">
          <p>OPEL</p>
        </Card>

        <Card id="card-10" draggable="true">
          <p>MAČICA</p>
        </Card>

      </Board>

    </main>
  </div>
</template>

<script>
import Board from './components/Board';
import Card from './components/Card';

export default {
  name: 'app',
  components: {
    Board,
    Card
  }
}
</script>

<style>

.naslov-strani {
  text-align: center;
}

.ime-stolpca-1 {
  color: white;
  text-align: center;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #f3f3f3;
}

.flexbox {
  display: flex;
  justify-content: space-between;

  width: 100%;
  max-width: 768px;
  height: 50vh;

  overflow: hidden;

  margin: 0 auto;
  padding: 15px;
}

.flexbox .board {
  display: flex;
  flex-direction: column;

  width: 100%;
  max-width: 300px;

  background-color: #313131;

  padding: 15px;
  border-radius: 5px;
}

.flexbox .board .card {
  padding: 15px 25px;
  background-color: white;
  border-radius: 5px;

  cursor: pointer;
  margin-bottom: 15px;
}
</style>
