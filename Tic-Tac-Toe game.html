<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic Tac Toe</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            font-family: 'Arial', sans-serif;
            color: white;
        }

        .game-container {
            text-align: center;
            padding: 20px;
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
        }

        h1 {
            font-size: 3em;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .board {
            display: grid;
            grid-template-columns: repeat(3, 100px);
            gap: 10px;
            background: rgba(255, 255, 255, 0.1);
            padding: 10px;
            margin: 20px auto;
            border-radius: 15px;
        }

        .cell {
            width: 100px;
            height: 100px;
            background: rgba(255, 255, 255, 0.1);
            border: none;
            border-radius: 10px;
            font-size: 50px;
            font-weight: bold;
            cursor: pointer;
            color: white;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .cell:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: scale(1.05);
        }

        .cell.pop {
            animation: pop 0.3s ease-out;
        }

        @keyframes pop {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        .status {
            font-size: 24px;
            margin: 20px 0;
            height: 40px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .winner {
            animation: winner 0.5s ease-in-out;
        }

        @keyframes winner {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        button.reset {
            font-size: 18px;
            padding: 12px 30px;
            cursor: pointer;
            background: rgba(255, 255, 255, 0.2);
            border: none;
            color: white;
            border-radius: 25px;
            transition: all 0.3s ease;
            margin-top: 20px;
        }

        button.reset:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
        }

        .cell[data-symbol="X"] {
            color: #FF6B6B;
        }

        .cell[data-symbol="O"] {
            color: #4ECDC4;
        }

        .winning-line {
            background-color: rgba(255, 255, 255, 0.2);
        }
    </style>
</head>
<body>
    <div class="game-container">
        <h1>Tic Tac Toe</h1>
        <div class="status" id="status">Player X's turn</div>
        <div class="board" id="board"></div>
        <button class="reset" onclick="resetGame()">Reset Game</button>
    </div>

    <script>
        let currentPlayer = 'X';
        let gameBoard = ['', '', '', '', '', '', '', '', ''];
        let gameActive = true;

        const board = document.getElementById('board');
        const status = document.getElementById('status');

        // Create board
        for (let i = 0; i < 9; i++) {
            const cell = document.createElement('button');
            cell.className = 'cell';
            cell.setAttribute('data-index', i);
            cell.addEventListener('click', () => handleClick(i));
            board.appendChild(cell);
        }

        function handleClick(index) {
            const cells = document.getElementsByClassName('cell');
            
            if (gameBoard[index] || !gameActive) return;

            gameBoard[index] = currentPlayer;
            cells[index].textContent = currentPlayer;
            cells[index].setAttribute('data-symbol', currentPlayer);
            cells[index].classList.add('pop');

            // Remove animation class after it's done
            setTimeout(() => {
                cells[index].classList.remove('pop');
            }, 300);

            if (checkWin()) {
                status.textContent = `Player ${currentPlayer} wins!`;
                status.classList.add('winner');
                gameActive = false;
                highlightWinningCells();
                return;
            }

            if (gameBoard.every(cell => cell !== '')) {
                status.textContent = "It's a draw!";
                status.classList.add('winner');
                gameActive = false;
                return;
            }

            currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
            status.textContent = `Player ${currentPlayer}'s turn`;
        }

        function checkWin() {
            const winPatterns = [
                [0, 1, 2], [3, 4, 5], [6, 7, 8],
                [0, 3, 6], [1, 4, 7], [2, 5, 8],
                [0, 4, 8], [2, 4, 6]
            ];

            return winPatterns.some(pattern => {
                return pattern.every(index => {
                    return gameBoard[index] === currentPlayer;
                });
            });
        }

        function highlightWinningCells() {
            const winPatterns = [
                [0, 1, 2], [3, 4, 5], [6, 7, 8],
                [0, 3, 6], [1, 4, 7], [2, 5, 8],
                [0, 4, 8], [2, 4, 6]
            ];

            const cells = document.getElementsByClassName('cell');
            
            winPatterns.forEach(pattern => {
                if (pattern.every(index => gameBoard[index] === currentPlayer)) {
                    pattern.forEach(index => {
                        cells[index].classList.add('winning-line');
                    });
                }
            });
        }

        function resetGame() {
            gameBoard = ['', '', '', '', '', '', '', '', ''];
            gameActive = true;
            currentPlayer = 'X';
            status.textContent = `Player ${currentPlayer}'s turn`;
            status.classList.remove('winner');
            
            const cells = document.getElementsByClassName('cell');
            for (let cell of cells) {
                cell.textContent = '';
                cell.setAttribute('data-symbol', '');
                cell.classList.remove('winning-line');
            }
        }
    </script>
</body>
</html>
