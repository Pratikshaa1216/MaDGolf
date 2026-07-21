<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/">
    <img src="https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/-/wikis/uploads/31a92f3dc70416b2f2cda0132a0474e0/Logo_black_101.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">MADgolf</h3>

  <p align="center">
    AI personalized golf coach, one click away!
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


## About The Project

 MaDGolf offers a mobile application that combines
Artificial Intelligence and Augmented Reality to provide real-time analytics and personalized assistance for golf enthusiasts.



    ✓ Personalised green mapping with drone and LiDar
    ✓ Train the AI model through Reinforcement Learning
    ✓ Visualize putt-path through application 



### Built With

* Software: Unity, Xcode
* Hardware: Drone, GoPro, LiDar Sensor, iPhone (LiDAR and AR)

<!-- CONTACT -->
### Contact
Contact us for questions, technical
assistance, or collaboration opportunities
via the contact information provided.

MadGolf: 
[Website](https://website-project-flax.vercel.app/) ,
[Email](madgolflab@gmail.com)

Project Link: [https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/](https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/)


<!-- GETTING STARTED -->
## Getting Started

### Setting Up the Project in Unity and Building for iOS

Follow the steps below to set up the Unity project from the Git repository and build it for iOS:

#### 1. Clone the Repository:
- Install git locally on your machine
- Set up git to connect to gitlab without annoying password (via ssh)
    1. `ssh-keygen -t ed25519 -b 4096`
    2. Upload generated public key to gitlab personal preferences in SSH keys section
    3. Edit local ~/.ssh/config (with hard tab stops) like below
    4. Clone with `git clone mad:InnoLab/ss24/golf-drone.git`

`~/.ssh/config`
```
Host mad
	Hostname mad-srv.informatik.uni-erlangen.de
	User git
	IdentityFile ~/.ssh/id_ed25519
```


#### 2. Open the Project in Unity:

- Launch Unity.
- In the Unity Hub, click on "Open".
- Navigate to the cloned repository folder and select it. Unity will open the project.

#### 3. Accessing the Scene:

-    Once the project is open, navigate to the Assets folder in the Unity Project window.
-    Open the specific scene you wish to work on by double-clicking the scene file.

#### 4. Build the Project for iOS:

-    Go to File > Build Settings in the Unity menu.
-    In the Build Settings window, select iOS as the target platform.
-    Click on the Build button.
-    Unity will prompt you to choose a location for the build output. Create a new directory within the Assets folder (e.g., iOSBuild) and select it as the output directory.
-    Unity will begin the build process. This may take some time.

#### 5. Open the Project in Xcode:

-    Once the build process is complete, locate the .xcodeproj file within the newly created directory inside the Assets folder.
-    Double-click on the .xcodeproj file to open the project in Xcode.

#### 6. Proceed with Xcode:

-    From here, you can configure the Xcode project as needed and proceed with further development, testing, or deployment.

<!-- USAGE EXAMPLES -->
## Project Structure
| Directory                         | Description                                                                                               |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------|
| `/Code/Model/Assets/`             | Code base for the whole project. Includes both Machine learning model and UI                               |
| `/Code/ui-golf/`                  | Code base for the UI standalone                                                                            |
| `/Planning/Ideation_April/`       | Documents for reference. Everything that was brainstormed by the team including logo, PPT, methodology, user story, and algorithm plans |
| `/Planning/MadGolf_video/`        | All the final videos: promotional advertisement and product                                                |
| `/Planning/drone_research/`       | Document regarding the research conducted before choosing and finalizing the drone to be used. Also includes all the images captured by the drone for the project |
| `/results/ppo/configuration.yaml` | YAML file for the configuration of the project. Also included                                              |
| `/results/ppo/RollerBall/`        | All the files required and used by the machine learning model behind the trajectory planning               |
 



<!-- USAGE EXAMPLES -->
## Usage
#### Below is the process structure of our app: 
<img src="https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/-/wikis/uploads/21964335e77d566d9ff35de94e05da47/approach.png" >



#### Here's the screen recorded video of using our our app: [Video](https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/-/blob/main/Planning/MadGolf_video/AppRecording.mov)


_For more examples on how to use the application, please refer to the [Wiki Documentation](https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/-/wikis/Documentation%20of%20the%20Software/UI)_



<!-- LICENSE -->
## License

Distributed under the Apache License Version 2.0. See `LICENSE.txt` for more information.



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

We would like to express our sincere gratitude to all those who have supported and contributed to this project.

Team Members and Product Owner: A big thank you to our dedicated team members who worked tirelessly to make this project a reality. Your expertise, hard work, and collaboration were invaluable. Also a big thankyou to Prof. Dr. Björn Eskofier and Mad Lab to give us this oppurtunity.

Scrum Master: We are deeply grateful to our Scrum Master Thomas , whose guidance and advice were crucial in navigating the complexities of technical tasks and project management.

Open Source Community: We extend our appreciation to the open-source community for providing the tools, libraries, and resources that significantly enhanced our project development.

Organization: We also acknowledge the support from InnoLab, which provided the resources and environment necessary for our research and development.

Testing and Validation Support: Special thanks to those who assisted with testing and validation, ensuring that our MadGolf drone project met all the necessary standards and requirements.

Friends and Family: Last but not least, we would like to thank our friends and families for their unwavering support and understanding throughout the course of this project.

This project would not have been possible without the collective efforts and contributions of all involved. We are excited about the future of this technology and look forward to continuing our work in this field.



Some resources that helped a lot to finish this project:
* [Research Article](https://www.researchgate.net/publication/237196126_The_physics_of_putting)
* [Unity Scripting Reference](https://docs.unity3d.com/ScriptReference/index.html)
* [Sequence Diagram](https://sequencediagram.org/)
* [More resources can be found on our wiki](https://mad-srv.informatik.uni-erlangen.de/InnoLab/ss24/golf-drone/-/wikis/home)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
