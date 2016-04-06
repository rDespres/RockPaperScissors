@echo off
cls



:idle
cls
echo.
echo.
echo.
echo.
echo.
echo                     ______                           _______
echo                    /      \__            	  __/       \
echo         __________/    ____^| ^|           	 ^| ^|____     \_____________
echo                       /______^|           	 ^|______\
echo                      /^|______^|          	 ^|______^|\
echo                       ^|______^|          	 ^|______^|   
echo         ________      ^|______^|          	 ^|______^|     _____________
echo                 \_____\_____/            	  \_____/____/
echo.
echo.
echo               1) Rock              2) Paper	    3) Scissors
                         


set /p input=CHOICE:
if %input%==1 goto Rock
if %input%==2 goto Paper
if %input%==3 goto Scissors


:Rock

set /a n=%random% %%3

if %n%==0 goto RockRock
if %n%==1 goto RockPaper
if %n%==2 goto RockScissors



:RockRock
cls

echo.
echo				     TIE!
echo.
echo.
echo.
echo                     ______            _______
echo                    /      \__      __/       \
echo         __________/    ____^| ^|    ^| ^|____     \_____________
echo                       /______^|    ^|______\
echo                      /^|______^|    ^|______^|\
echo                       ^|______^|    ^|______^|   
echo         ________      ^|______^|    ^|______^|     ___________
echo                 \_____\_____/      \_____/____/
 

timeout /T 2 >nul
goto idle



:RockPaper
cls

echo.
echo				      LOSS!
echo.
echo.
echo.          
echo                     ______                   _______
echo                    /      \__        _______/       \
echo         __________/    ____^| ^|      ^|_____ ^|____     \_____________
echo                       /______^|     ^|______      \
echo                      /^|______^|      ^|_____       
echo                       ^|______^|       ^|_____        ________________
echo         ________      ^|______^|         \__________/              
echo                 \_____\_____/                    




timeout /T 2 >nul
goto idle


:RockScissors
cls

echo.
echo				      WIN!
echo.
echo.
echo.
echo                     ______                   _______
echo                    /      \__       ________/       \
echo         __________/    ____^| ^|     ^|_______^|____     \_____________
echo                       /______^|      _______\    \
echo                      /^|______^|     ^|____________ \
echo                       ^|______^|           ^|______^|   
echo         ________      ^|______^|           ^|______^|     ___________
echo                 \_____\_____/             \_____/____/



timeout /T 2 >nul
goto idle




:Paper

cls
set /a n=%random% %%3

if %n%==0 goto PaperRock
if %n%==1 goto PaperPaper
if %n%==2 goto PaperScissors




:PaperRock
cls

echo.
echo				            WIN!
echo.
echo.
echo.
echo                     ______                         _______
echo                    /      \________             __/       \
echo         __________/    ____^| ______^|           ^| ^|____     \_____________
echo                       /      _______^|          ^|______\
echo                      /       ______^|           ^|______^|\
echo         _________           ______^|            ^|______^|    
echo                  \______________/              ^|______^|     ___________
echo                                                 \_____/____/



timeout /T 2 >nul
goto idle


:PaperPaper
cls

echo.
echo				            TIE!
echo.
echo.
echo.
echo                     ______                         _______
echo                    /      \________        _______/       \
echo         __________/    ____^| ______^|      ^|______ ^|___     \_____________
echo                       /      _______^|    ^|_______     \
echo                      /       ______^|      ^|______      \
echo         _________           ______^|        ^|______          _____________
echo                  \______________/            \_____________/            



timeout /T 2 >nul
goto idle



:PaperScissors
cls

echo.
echo				        LOSS!
echo.
echo.
echo.         
echo                     ______                        _______
echo                    /      \________      ________/       \
echo         __________/    ____^| ______^|    ^|______ ^|____     \_____________
echo                       /      _______^|    ______\     \
echo                      /      _______^|    ^|____________ \
echo         _________           ______^|           ^|______^|   
echo                  \_____________/              ^|______^|     ___________
echo                                                \_____/____/


timeout /T 2 >nul
goto idle


:Scissors

cls
set /a n=%random% %%3

if %n%==0 goto ScissorsRock
if %n%==1 goto ScissorsPaper
if %n%==2 goto ScissorsScissors


:ScissorsRock
cls

echo.
echo				        LOSS!
echo.
echo.
echo.
echo                     ______                    _______
echo                    /      \_________       __/       \
echo         __________/    ____^| _______^|     ^| ^|____     \_____________
echo                       /     /_______      ^|______\
echo                      / _____________^|     ^|______^|\
echo                       ^|______^|            ^|______^|   
echo         ________      ^|______^|            ^|______^|     ___________
echo                 \_____\_____/              \_____/____/


timeout /T 2 >nul
goto idle


:ScissorsPaper
cls

echo.
echo				           WIN!
echo.
echo.
echo.
echo                     ______                        _______
echo                    /      \________       _______/       \
echo         __________/    ____^| ______^|     ^|_____ ^|____     \_____________
echo                       /     /______     ^|______      \
echo                      /^|____________^|     ^|_____       
echo                       ^|______^|            ^|_____        ________________
echo         ________      ^|______^|              \__________/              
echo                 \_____\_____/   

timeout /T 2 >nul
goto idle


:ScissorsScissors
cls

echo.
echo				           TIE!
echo.
echo.
echo.
echo                     ______                         _______
echo                    /      \_________      ________/       \
echo         __________/    ____^| _______^|    ^|______^|____     \_____________
echo                       /     /_______      ______\     \
echo                      / _____________^|    ^|____________ \
echo                       ^|______^|                 ^|______^|   
echo         ________      ^|______^|                 ^|______^|     ___________
echo                 \_____\_____/                   \_____/____/        


timeout /T 2 >nul
goto idle        

