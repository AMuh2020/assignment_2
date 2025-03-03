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