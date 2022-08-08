Author: Basma Elhoseny

# 8086-Microprocessor-Game
It is a game based on the 8086 Microprocessor played by 2 players against each other. The winner is the one who can put the value “105e” in any of the opponent registers. 

The main file to run g.exe. Each player has to run this file to start the game. The connection can be done using a virtual serial port on the same machine or using a TTL wired connection between two different PCs.

---------------------------------------------------------------------------------------------------------------------------------------------------------------
Each player enters his name and the suggested initial points he wants and the final points with which each player starts are the less between those suggested by the two players.
The user name should be not more than 15 characters and start with a letter, not a digit or a special character.

---------------------------------------------------------------------------------------------------------------------------------------------------------------
Chatting Mode:
Before starting the game there is a feature of chatting with the other player. All you have to do is to send an invitation to your opponent and keep waiting for his acceptance.

The chating has a scroll feature automatically when no space on the screen.

-------------------------------------------------------------------------------------------------------------------------------------------------------------
Game: To start the game one of the players sends an invitation to the other and keeps waiting for acceptance.
Note: All these actions are shown in a notification bar a the bottom of the screen
we have two levels. chosen by the sender of the game invitation.

The inline chat feature is available during the game.

Level1:
- Each player chooses a forbidden alphanumeric character (0 – 9 A-Z) that the opponent can’t use for any command.
- The player who sent the invitation starts with the first command. The command written by the first player executes on the other player's processor.
- The opponent should prevent this by the initial forbidden character or special power-ups. 

-------------------------------------------------------------------------------------------------------------------------------------------------------------
Level2:
Exactly like level1 by with some extra features
  - hidden forbidden character
  - could select whether to perform this command on your processor or the opponent's processor
  - initial values for registers.
  
-------------------------------------------------------------------------------------------------------------------------------------------------------------
Special Powers(in levels 1 & 2): each player has a specfic no of special powers that he can use
  - Clear all the registers at once. (Consumes 30 points and could be used only once).
  - Making one of the data lines stuck at zero or one for a single instruction (consumes 2 points).
  - Executing a command on your processor (consumes 5 points).
  - Executing a command on your processor and your opponent processor at the same time (consumes 3 points).

------------------------------------------------------------------------------------------------------------------------------------------------------------
Errors are detected either size mismatch or invalid instruction in assembly causing you to lose points.

------------------------------------------------------------------------------------------------------------------------------------------------------------
Instructions encoding:
0==>MOV
1==>nop
2==>clc
3==>inc
4==>dec
5==>shl
6==>shr
7==>push
8==>pop
9==>ror
a==>rol
b==>rcr
c==>rcl
d==>sar
e==>mul
f==>div
g==>imul
h==>idiv
i==>add
j==>sub

----------------------------------------------------------------------------------------------------------------------------------------------------------
Registers Encoding:
I==>AX
K==>BX
M==>CX
O==>DX
a==>AH
b==>AL
c==>BH
d=>BL
e==>CH
f==>CL
g==>DH
h==>DL
A==>SI
C==>DI
E==>SP
G==>BP

----------------------------------------------------------------------------------------------------------------------------------------------------------
Memory Encoding:
B==>[SI]
D==>[DI]
R==>[BX]
i==>[00]
j==>[01]
k==>[02]
l==>[03]
m==>[04]
n==>[05]
o==>[06]
p==>[07]
q==>[08]
r==>[09]
s==>[0A]
t==>[0B]
u==>[0C]
v==>[0D]
w==>[0E]
x==>[0F]
