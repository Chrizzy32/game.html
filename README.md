# game.html

<!DOCTYPE html>
<html>
<head>
    <title>Text Adventure Game</title>
</head>
<body>
    <h1>Haunted House Adventure</h1>
    <p>You find yourself standing in front of a spooky haunted house. What do you do?</p>
    <ul>
        <li><a href="#explore">Explore the house</a></li>
        <li><a href="#run">Run away</a></li>
    </ul>

    <div id="explore" style="display: none;">
        <p>You enter the house and find a dark hallway. There are two doors, one on the left and one on the right. Which do you choose?</p>
        <ul>
            <li><a href="#left">Go left</a></li>
            <li><a href="#right">Go right</a></li>
        </ul>
    </div>

    <div id="run" style="display: none;">
        <p>You turn and run as fast as you can, but you trip and fall. Suddenly, you feel a cold hand on your shoulder...</p>
    </div>

    <div id="left" style="display: none;">
        <p>You enter a dusty old library. There's a book on the table. Do you open it?</p>
        <ul>
            <li><a href="#open">Open the book</a></li>
            <li><a href="#leave">Leave the library</a></li>
        </ul>
    </div>

    <div id="right" style="display: none;">
        <p>You find yourself in a creepy dining room. The table is set for a meal, but there's no one around. What do you do?</p>
        <ul>
            <li><a href="#eat">Sit down and eat</a></li>
            <li><a href="#leave">Leave the room</a></li>
        </ul>
    </div>

    <div id="open" style="display: none;">
        <p>As you open the book, a ghostly figure appears and says, "Congratulations, you've found the treasure!" You win!</p>
    </div>

    <div id="eat" style="display: none;">
        <p>As you take a bite of the food, you start to feel strange. You collapse to the floor and everything goes black...</p>
    </div>

    <div id="leave" style="display: none;">
        <p>You decide to leave the room and head back outside. As you walk away, you hear a voice whisper, "Come back soon..."</p>
    </div>

    <script>
        function showSection(id) {
            // Hide all sections
            var sections = document.querySelectorAll('div');
            for (var i = 0; i < sections.length; i++) {
                sections[i].style.display = 'none';
            }
            // Show the selected section
            document.getElementById(id).style.display = 'block';
        }
    </script>
</body>
</html>
