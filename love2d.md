# Love2D

## Methods
| Command         | Description                       |
|-----------------|-----------------------------------|
| love.draw()     | Called every gameloop             |
| love.update(dt) | Called every frame                |
|                 | dt = delta - time since last loop |
| love.load()     | Called once at beginning of app   |
| love.quit()     | Called as cleanup                 |
|                 |                                   |

# Setup
- conf.lua

| Command            | Description                     |
|--------------------|---------------------------------|
| love.conf(t)       | conf.lua takes this function    |
|                    | t = table                       |
| t.window.title     | The title of the window         |
| t.window.width     | Width of the window             |
| t.window.height    | Height of the window            |
| t.modules.<module> | Switch modules on/off (boolean) |

(Config Reference)[https://love2d.org/wiki/Config_Files]
