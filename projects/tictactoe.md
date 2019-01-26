---
layout: project
type: project
image: images/tictactoe.png
title: 3D Tic-Tac-Toe
permalink: projects/project-tictactoe
# All dates must be YYYY-MM-DD format!
date: 2018-05-03
labels:
  - Linux
  - SFML
  - C++
summary: My team developed a 3D Tic-Tac-Toe Game using C+\+ in a Linux Environment
---

The snippet of code below shows how the pieces are originally set onto the gameboard upon startup.

```c++
Piece::Piece(float posX, float posY){
    // O Texture
    otexture.setSmooth(true);
    otexture.loadFromFile("res/images/O.png");
    // X Texture
    xtexture.setSmooth(true);
    xtexture.loadFromFile("res/images/X.png");

    for (int x = 0; x < 3; x++)
    {
        for (int y = 0; y < 3; y++)
  		{
            piece[x][y].setScale(BSCALE,BSCALE);
            piece[x][y].setTexture(otexture);

            // Change last value to 0 in order to make pieces invisible
            piece[x][y].setColor(sf::Color(255, 255, 255, 0));
            // the -2 is needed to center the Piece
            piece[x][y].setPosition(posX + (PSIZE * x) - 2, posY + (PSIZE * y) - 2);
        }
    }
}
```


