# cmnz71 Programming Black assignment 2 log

## pre-something

A few other programming black students and I decided to use our ongoing work with the Durham robotics society to use for assignment 2. We've already spent several weeks discussing, planning and now testing/implementing our idea to see how feasible it is. The Log begins approximately 6 weeks into this. Each session is 2 hours each, from 6-8pm every thursday.

Our project goal is to eventually develop a autonomous shopping cart to help the elderly and people with other disabilities to shop easier and better. The shopping cart will be able to follow the shopper at a small distance and always be at hand to take their items. It'll be interfaced by custom software (made by us eventually) so that it knows exactly where it is in the supermarket and where other shopping carts are to avoid collisions. It'll also have a local sensor array, consisting of a Lidar, for enviroment scanning, a IMU for positioning and a camera for object and collision detection. The local sensor array will all be brought together into implementing a SLAM algorithm running locally on the robot (hence a Jetson Nano), to enable autonmous manuverability, detection, and an awareness of its surroundings, ensuring a safe and easy experience for shoppers.

## Entry #1
Late LOG 20/02/2025 written 25/02/2025 (and 03/03/2025)

Today we worked on setting up the nvidia jetson nano 2gb. In last weeks session I had already began this process my flashing the jetsons Operating system (Jetpack something something) onto an old 64gb SD card I had on hand. I first had to copy the data on it, I believe the sd card was previously used by my father in one of his old phones, which took about an 1 hour, and then install and flash the OS onto it, which took another 20-30 mins. This week my team and I finally got the Nano booted up and working, however we had a lot of issues with the wifi, as the ARM (something something) processor on the board didnt come with a wifi (chip?). We spent the next two hours fiddling around and researching how we could get it to connect to the internet, to no avail. We were able to interface with the board through PuTTy's serial monitor via a USB cable through what Nvidia call, headless mode, as the jetson nano is capable of supporting a hdmi connection and thus a display and interface just like a normal computer. We went with headless mode because we didnt have a monitor on hand.

Another notable event that happened today was the arrival of our teams equipment we had ordered from RS (finally!). Due to the strict budget set by the society, we were limited in what we could acquire. Our purchases included a small LiDar sensor, and a board + cable to convert the lidars pinout to usb (editors note, this would turn out to not be needed....) and a quite pricy (16 pounds!) IMU (Inerital Measurement Unit).

## Entry #2
27/02/2025

Another team is building an almost exact model of the robot we want to build, although their use case will be different so our code and actual final build will be different. The team is made up of much more knowledgable second years so, after kindly asking them if they could show us some stuff, we spent the session working with them. Unlike our team they are able to take thier jetson nano home with them and thus are quite far ahead. They already have a camera and lidar (we have the exact same lidar coincidently), and are able to get a nearly live camera feed on thier computer using rerun.io a "log handling and visualisation software".

Thier team helped us setup our jetson nano, running us through the setup process and connecting the raspberry pi camera. We learned what our next steps should be an will be working towards getting our own system set up soon so we can start testing the if our idea can come together (or if we need more sensors).

## Entry #3
06/03/2025

There was no session today so the team and I decided to do some research on our own time this week. I decided to look into how the robot would look like, looking at similar examples online in terms of functionality. We are currently looking at a 3 or 4 wheeled robot that can be manueveured using

look rosviz and learnt about ROS and how it could

## Entry #4
20/03/2025, completed 06/04/2025

There werent any sessions for the last two weeks as the robotics soc heads were busy with coursework, however there was one today. We worked on trying to get camera access, and after a few unsuccesful attempts we turned to chatgpt, which then lead to many more unsuccesful attempts. One of us on the team also had an issue connecting to the jetson nano through ssh, it turned out one of thier ssh keys was the default one and whenever they tried to ssh it used that instead of the one he made (he forgot the password of the previous key), eventually after 20 minutes of trial and error we just went with deleting all his previous keys, and generating a new one which eventually worked. We also had issues testing the camera as the nano was in headless mode, and there arent many ways to test it. Before the end of the session we figured out multiple ways forward which we shall be testing in the next session. This is also the final session of the term, my group and I will try and meet up over the break virtually at least once before exams to discuss our plans going forward and do a little research.