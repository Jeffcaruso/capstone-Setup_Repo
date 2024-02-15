# CSS 342 / 343 Docker Setup

## Purpose
This repository is intended to support you configuring your Docker container to use Google Test to support your Test Driven Development

## Steps for you to follow for Setup of gTest
1. Setup container following [CSS Wiki Instructions](https://csswiki.uwb.edu/css-linux-lab-docker-image/)
    1. NOTE: You will need to sign in with your UW NET ID 
1. Add the extensions to VSC that are listed in the "Steps for additional dependencies" section below
1. CSS Wiki on how to [open Docker container](https://csswiki.uwb.edu/attach-vscode-to-csslab-docker-container/)
    1. NOTE: You will need to sign in with your UW NET ID 
    1. Docker - start the container you made from containers page of docker desktop
    1. Remote Explorer (VSC) - find the container with the play button icon
    ![images/play button.png](https://github.com/Jeffcaruso/capstone-Setup_Repo/blob/main/images/play%20button.PNG))
    1. Open the container (pick either A or B)
        1. Same window - press arrow; ->
        1. New window, the window with a + in corner; +[]
        ![images/showing opening](https://github.com/Jeffcaruso/capstone-Setup_Repo/blob/main/images/showing%20area%20selected.png)
    1. Wait for loading (probably will say something like 'starting container' and have a loading bar)
1. Clone the repo e.g.,'git clone https://github.com/Jeffcaruso/capstone-Setup_Repo.git'
1. Enter command in bash terminal: 'cd capstone-Setup_Repo/'
1. Enter command in bash terminal: './install-googletest.sh'
    1. NOTE: install-googletest.sh should be executable, but if for some reason that gets lost, Enter command in bash terminal: 'chmod +x install-googletest.sh'; Then run install command again
1. Wait for the script to run and install google test
1. Following notes at bottom of script,
    1. If install ok (no errors), Enter command in bash terminal: 'rm -rf googletest'
    2. If not ok (errors), follow instrucitons left at end of the output, seek additional support if needed.
1. Verify that the extensions found in the "Steps for additional dependencies" below are installed on the container
    1. Those should be present in both of the following:
        1. Local - Installed
        1. Container CSSIMAGES/MULTIARCH:LATEST
1. Congratulations! Google Test should now be installed!
    1. You will not have to run the install script again locally within the contatiner used. You will only need to re-do this process to use a different container
    2. The install script (install-googletest.sh) will be present in future repos for GitHub Actions' usage. You will not need to use it or intervene to install google test on GitHub Actions

## Steps for additional dependencies
add the following extensions:
- Remote Development (should have from Step 2 above)
- C/C++
- C/C++ extension pack
    - Automatically installs: CMake, CMake Tools, C/C++ Themes 
Resulting Extensions should include (more ok, but at least these):
![Extensions You Should have](https://github.com/Jeffcaruso/capstone-Setup_Repo/blob/main/images/extensions%20view.PNG)
