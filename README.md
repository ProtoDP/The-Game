#Platformer Game
## Description
Basic platformer with jumping , crouching , sprinting and wallrunning and jumping 
### Demo
![image](https://github.com/user-attachments/assets/d2c57d3f-0995-4f00-be94-058a814fb5ea)


# Tech
-C#
-Unity game engine 
-Clion Ide
Unique features
-Wallrunning and walljumping 
-crouching
-gravity using Character controller
# Download adn installation
Download the game files labeled "The Game" and start TheGame.exe
# Script descriptors
## -Movement.cs
### Start().	
Void	Сохраняет исходные параметры роста игрока и камеры, чтобы правильно работать с приседанием
### CheckWall()	
Void	Проверяет, находятся ли стены слева или справа от игрока для возможности бегать по стенам.
### Update()	
 void	•	Основной цикл управления движением: проверка земли, бег, прыжки, приседание, бег по стенам, обработка гравитации, наклон камеры и переход между состояниями.
## -CamFPS.cs
### Start()
	void	Прячет курсор и блокирует его в центре экрана для имитации поведения камеры от первого лица.
### Update()
	void	Обрабатывает вращение камеры на основе движения мыши и вращает объект orientation по горизонтали.
## -Gamedm.cs
### Start()	Void	Выключает надписи «Game Over» и «You Win» при запуске.
### Update()	void	Если игра окончена, ожидает нажатия любой клавиши для перезапуска или выхода (если победа).
### GameOver()	Void	Активирует режим проигрыша и отображает сообщение об окончании игры.
### GameWin()	void	Активирует режим победы и отображает соответствующее сообщение.
### RestartGame()	void	Перезагружает текущую сцену.
## -Thebigwin.cs/ Thebigdie.cs
### OnTriggerEnter(Collider other)	Void	Если игрок входит в триггер с тегом kiw, вызывает окончание игры (GameOver()).
### OnTriggerEnter(Collider other)	void	Если игрок входит в триггер с тегом wiw, вызывает победу в игре (GameWin()).



