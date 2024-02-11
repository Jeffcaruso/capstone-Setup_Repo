# CSS 342 / 343 Docker Setup

## Steps for you to follow for Setup
1. Setup container following [CSS Wiki Instructions](https://csswiki.uwb.edu/css-linux-lab-docker-image/)
    1. NOTE: You will need to sign in with your UW NET ID 
1. CSS Wiki on how to [open Docker container](https://csswiki.uwb.edu/attach-vscode-to-csslab-docker-container/)
    1. NOTE: You will need to sign in with your UW NET ID 
    1. Docker - start the container you made from containers page of docker desktop
    1. Remote Explorer (VSC) - find the container with the play button icon
   ![title](Images/example.png)
    1. Open the container (pick either A or B)
        1. Same window - press arrow; ->
        1. New window, the window with a + in corner; +[]
    1. Wait for loading (probably will say something like 'starting dev container')
1. 'git clone https://github.com/Jeffcaruso/capstone-Setup_Repo.git'
1. 'cd capstone-Setup_Repo/'
1. //NOTE: install-googletest.sh should be executable, but if for some reason that gets lost, do a chmod +x
1. './install-googletest.sh'
1. Wait for the script to run and install google test
1. Following notes at bottom of script, If install ok (no errors), do 'rm -rf googletest'
1. Congratulations! Google Test should now be installed!
