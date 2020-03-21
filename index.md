<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Trivial Pursuit: Covid Death Spiral Edition</title>

    <link rel="stylesheet" type="text/css" href="css/normalize.css">
    <link rel="stylesheet" type="text/css" href="css/gamepieces.css">
    <link rel="stylesheet" type="text/css" href="css/wedges.css">
    <link rel="stylesheet" type="text/css" href="css/game.css">

</head>
<body>
  <div id="window-container">
    <div id="game-container">

        <div id="board-left" style="padding-top: 100px;">
            <img id="logo" class="noselect" src="images/tpelogo.png" alt="" />

            <br />

            <table id="score-table">
                <tr>
                    <th>Teams</th>
                    <th>
                        <span id="w0" class="wedge wedge0" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w1" class="wedge wedge1" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w2" class="wedge wedge2" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w3" class="wedge wedge3" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w4" class="wedge wedge4" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w5" class="wedge wedge5" draggable="true" data-draggable="master-wedge">&#9660;</span>
                    </th>
                </tr>
                <tr><td contenteditable="true" style="color:cornflowerblue">Player 1</td>  <td id="t0"></td></tr>
                <tr><td contenteditable="true" style="color:darkorange">Player 2</td>    <td id="t1"></td></tr>
                <tr><td contenteditable="true" style="color:deeppink">Player 3</td>       <td id="t2"></td></tr>
                <tr><td contenteditable="true" style="color:green">Player 4</td>         <td id="t3"></td></tr>
                <tr><td contenteditable="true" style="color:gold">Player 5</td>          <td id="t4"></td></tr>
                <tr><td contenteditable="true" style="color:red">Player 6</td>              <td id="t5"></td></tr>
            </table>

            <br />

            <table id="dice-table">
                <tr>
                    <td><script type="text/javascript">
                        D6.setBaseUrl('dice-roller/');
                        D6.dice(1);
                        D6.setButtonLabel('Roll the dice!');
                        $('.die').css('width', '80px');
                        D6.roll();
                    </script></td>
                </tr>
            </table>

            <br />
            <a class="left-link" href="howtoplay.html">How to play</a><br/>
            <a class="left-link" href="https://github.com/mb4828/trivialpursuit">Adapted From & Inspired By</a>

        </div>

        <div id="board-right" style="margin-top: 0px;">
            <img id="board" class="noselect" style="width: 80%;" data-draggable="target" src="images/trivpur2.png" alt="" />

            <table id="pieces-table">
                <tr>
                    <td><div id="p0" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:cornflowerblue;background-image: url(images/ed-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                    <td><div id="p1" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:darkorange;background-image: url(images/slein-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                    <td><div id="p2" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:deeppink;background-image: url(images/doug-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                    <td><div id="p3" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:green;background-image: url(images/newman-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                    <td><div id="p4" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:gold;background-image: url(images/selmont-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                    <!-- <td><div id="p5" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:red"></div></td> -->
                </tr>
            </table>

            <!--<img id="p0" class="gamepiece" draggable="true" data-draggable="gp" src="images/p0.png" alt="" />
            <img id="p1" class="gamepiece" draggable="true" data-draggable="gp" src="images/p1.png" alt="" />
            <img id="p2" class="gamepiece" draggable="true" data-draggable="gp" src="images/p2.png" alt="" />
            <img id="p3" class="gamepiece" draggable="true" data-draggable="gp" src="images/p3.png" alt="" />
            <img id="p4" class="gamepiece" draggable="true" data-draggable="gp" src="images/p4.png" alt="" />
            <img id="p5" class="gamepiece" draggable="true" data-draggable="gp" src="images/p5.png" alt="" />-->
        </div>

    </div>
  </div>

  <script type="text/javascript" src="scripts/jquery-2.1.4.min.js"></script>
  <script type="text/javascript" src="scripts/gamescripts.js"></script>
  <script type='text/javascript' src='dice-roller/d6.js'></script>

</body>
</html>
