<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Expendables Trivial Pursuit</title>

    <link rel="stylesheet" type="text/css" href="css/normalize.css">
    <link rel="stylesheet" type="text/css" href="css/gamepieces.css">
    <link rel="stylesheet" type="text/css" href="css/wedges.css">
    <link rel="stylesheet" type="text/css" href="css/game.css">

</head>
<body>
  <div id="window-container">
    <div id="game-container">

        <div id="board-left" style="padding-top: 40px;">
            <img id="logo" class="noselect" src="images/tpelogo.png" alt="" />

            <br />

            <table id="score-table">
                <tr>
                    <th>Teams</th>
                    <th>Score</th>
                    <th>
                        <span id="w0" class="wedge wedge0" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w1" class="wedge wedge1" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w2" class="wedge wedge2" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w3" class="wedge wedge3" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w4" class="wedge wedge4" draggable="true" data-draggable="master-wedge">&#9660;</span>
                        <span id="w5" class="wedge wedge5" draggable="true" data-draggable="master-wedge">&#9660;</span>
                    </th>
                </tr>
                <tr><td style="color:cornflowerblue">Mr. & Mrs. K</td><td>0</td>  <td id="t0"></td></tr>
                <tr><td style="color:darkorange">Stenton Survivors</td><td>0</td>    <td id="t1"></td></tr>
                <tr><td style="color:deeppink">Allie & Phil</td><td>0</td>        <td id="t2"></td></tr>
                <!-- <tr><td style="color:green">Newmanator</td><td>0</td>          <td id="t3"></td></tr>
                <tr><td style="color:gold">Selmont</td><td>0</td>          <td id="t4"></td></tr>
                <tr><td style="color:red"></td>              <td id="t5"></td></tr> -->
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

            <table id="card-table">
                <tr><td style="background-color:#0000FF; color:#000;">Geography</td></tr>
                <tr><td style="background-color:#FF75C3; color:#000;">Entertainment</td></tr>
                <tr><td style="background-color:#FFFF00; color:#000;">History</td></tr>
                <tr><td style="background-color:#92278F; color:#000;">Art & Literature</td></tr>
                <tr><td style="background-color:#04C71F; color:#000;">Science & Nature</td></tr>
                <tr><td style="background-color:#F26522; color:#000;">Sports & Leisure</td></tr>
            </table>

        </div>

        <div id="board-right">
            <img id="board" class="noselect" data-draggable="target" src="images/trivpur2.png" alt="" />

            <table id="pieces-table">
                <tr>
                <td><div id="p0" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:cornflowerblue;background-image: url(images/mr-mrs-icon.png); background-repeat:no-repeat;background-position: center center; height: 80px; width: 80px; background-size: 80px 80px;"></div></td>
                <td><div id="p1" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:darkorange;background-image: url(images/mike-beth-icon.png); background-repeat:no-repeat;background-position: center center; height: 80px; width: 80px; background-size: 80px 80px;"></div></td>
                <td><div id="p2" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:deeppink;background-image: url(images/al-phil-icon.png); background-repeat:no-repeat;background-position: center center; height: 80px; width: 80px; background-size: 80px 80px;"></div></td>
                <!--  <td><div id="p3" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:green;background-image: url(images/newman-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                <td><div id="p4" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:gold;background-image: url(images/selmont-icon.png); background-repeat:no-repeat;background-position: center center; height: 60px; width: 60px; background-size: 70px 70px;"></div></td>
                <td><div id="p5" class="gamepiece" draggable="true" data-draggable="gamepiece" style="background-color:red"></div></td> -->
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
