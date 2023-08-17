# ISB3DPRINTERS Solution In Progress (Aug 16 '23)

While we (barely) managed to get though the '23 school year with the current 3d printing soltuion, it's far from ideal. The accepted solution was to use a SBC to host a website for the ISB 3d printers project. Going into this I knew that it would ba a learning curve. At the moment I'm just testing out what needs to be built and learning through the documentation of required software.


Here's where I'm at now:

**Sites:**

  Docker
  
    -octoprint1 @ :8001
    
    -octoprint2 @ :8002
    
    -octoprint3 @ :8003
    
    -octoprint4 @ :8004
  
  Nodejs as system service (integrates with the automated-server)
    
    -teacherspage @ :8005

      -Password locked
    
**Other:**

HAProxy
  
  -turns all ports into paths (etc :8001 --> /printer1)

Automated-server
  
  -Runs as a node.js system service
  
  -Why? Because I'm comfortable and on a time constraint. No I'm not gonna do python :|
  
  -It is scheduled
  
  -This updates the passwords using Octoprints API

  -The passwords are stored on the computer and accessed by the Teachers site

Remote.it

  -Allows me and added contributers to work on it/debug from anywhere with full access

  -May move to using pitunnel or just developing my own remote tunnel

Portainer

  -Runs in docker
  
  -Makes it easier to modify docker settings

  -Will be removed as soon as not useful


## Goals:

Eventually this project will be fully opensource. This project may not be done till end of '23, I'm probably going to use this as my stem expo since it's not a small project. There will likely be a second computer, also opensource, jsut for management purposes.

## Physical Goals:

Indeed I have goals for more then just the software function of this, I'll probably bring a few power tools and build a little plexiglass console, with a little cli screen and small keyboard aswell as ventilation, of course not damaging the walls or anything. Just a little self contained terminal. I'll also probably run a removable quarter round cable hider for the microUSBs.
