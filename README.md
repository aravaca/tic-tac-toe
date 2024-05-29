# About Tic-tac-toe

This project includes a classic 3x3 tic-tac-toe game where you play against an unbeatable AI computer. The algorithm was designed based on Newell and Simon's 1972 tic-tac-toe model.<br/>
(KOR) 이 프로젝트는 3x3 틱택토 게임에서 절대 지지 않는 인공지능 컴퓨터를 구현합니다. 뉴웰과 사이먼의 1972 틱택토 모델을 바탕으로 알고리즘을 제작하였습니다.

## Basic Rules

<img src="https://github.com/aravaca/tic-tac-toe/assets/157980478/181351bb-eb24-40f3-bfb3-2b71541fc30b" width="120">

Two players take turns putting their marks (either X or O) in empty squares. The first player to get 3 of their marks in a row (up, down, across, or diagonally) is the winner. Tic-tac-toe is a classic zero-sum game meaning that winning of a player automatically leads to losing of the other player. If that is not the case, it's a tie. <br/>
두 명의 선수가 돌아가며 3x3 판 위 빈 사각형에 자신의 말(X 또는 O)을 넣습니다. 자신의 말 중 3개를 연속으로 연결시킨 첫 번째 선수가 승자입니다. 틱택토는 한 선수의 승리가 자동으로 다른 선수의 패배로 이어진다는 의미에서 고전적인 제로섬 게임입니다. 만약 누구 한 명이라도 이기거나 지지 않는다면 경기는 무승부입니다.

## How does the AI work?

The AI uses an algorithm that looks ahead a couple of moves and classifies all available moves in terms of priority. The AI will choose a move with the highest assigned priority to the extent that it does not present an opportunity for the human player to win. This allows the AI to tie in with the human player in the worst case. <br/>
인공지능은 몇 수 앞을 내다보고 사용 가능한 모든 수를 우선 순위 측면에서 분류하는 알고리즘을 사용합니다. 인공지능은 인간 플레이어가 이길 수 있는 기회를 제시하지 않는 범위에서 가장 높은 우선 순위를 가진 수를 선택할 것입니다. 이것은 최악의 경우 인공지능이 인간 플레이어와 동점을 이루도록 합니다.

## Description

To play the game on Windows, simply download and run the game.exe file in the dist folder. On other operating systems, assuming that you have Python installed, clone the repository and run the game using the following command in the terminal:<br/>
Windows에서 게임을 하려면 dist 폴더에서 game.exe 파일을 다운로드하여 실행하기만 하면 됩니다. 다른 운영 체제에서는 Python이 설치되어 있다고 가정하에, repository를 복제하고 터미널에서 다음 명령을 사용하여 게임을 실행합니다.<br/>
```bash
git clone https://github.com/aravaca/tic-tac-toe
cd tic-tac-toe\
python game.py
```
Then, follow the instructions as you play on the console.<br/>
그런 다음 콘솔에서 플레이하며 게임 안내를 따르면 됩니다.

NOTE:
The grid uses 1-9 indexing from left to right in the following form:<br/>
판은 다음과 같은 형태로 왼쪽에서 오른쪽으로 1-9 인덱싱을 사용합니다. <br/>
1 | 2 | 3<br/>
4 | 5 | 6<br/>
7 | 8 | 9<br/>

## Acknowledgement
The source code for the basic version of the game is from Kylie Ying's GitHub (https://github.com/kying18). I want to give a special thanks to her YouTube tutorial. However, elements like class AI_Player in player.py, method get_owl and check_two_in_row in game.py, and the main method that contain all necessary logic and procedures for the AI and its algorithm are solely written on my own. I have also added features such as a scoreboard, choosing the order for which player goes first, and playing multiple times. For the perfect tic-tac-toe algorithm, I referred to K.Crowley and R.Siegler's research paper *Flexible Strategy Use in Young Children’s Tic-Tac-Toe* (Carnegie Mellon University, 1993).<br/>
게임의 기본 버전 소스 코드는 카일리 잉(Kylie Ying)의 깃허브(https://github.com/kying18) 에서 가져온 것입니다. 그녀의 유튜브 튜토리얼에 특별한 감사를 표하고 싶습니다. 그러나 player.py 의 AI_Player 클래스, game.py 의 method get_owl 및 check_two_in_row, 그리고 메인 메소드 등 AI와 그 알고리즘에 필요한 모든 논리와 절차가 포함된 구성 요소는 전적으로 스스로의 힘으로 작성되었습니다. 스코어보드, 선공 순서 선택, 여러 번 플레이 등의 기능도 추가했습니다. 완벽한 틱택토 알고리즘을 구현하기 위해 K.Crowley와 R.Siegler의 논문 *Flexible Strategy Use in Young Children’s Tic-Tac-Toe*(카네기 멜론 대학, 1993년)을 참고했습니다.


