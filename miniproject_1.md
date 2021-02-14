a. Was your social distance detector effective at detecting potential violations? Are you able to describe how the distance detector is applying its calculations of either being safe or noting a violation?

It seemed to be relatively effective, there were definetely sometimes that the detector could not discern distance from a a depth perspective and others when people next to each other had green squares. The image processing function seems to be discerning that the shapes in the video are humans, and then assigning centroids to them. Then the Check function calculates the distance and returns either false or true to determine if it is distanced.

b. Do you think this approach would be effective for estimating new infections in real time? How would you implement such an approach in response to the COVID-19 pandemic we are currently experiencing?

It seems it would be relatively effective, but one of the main components of COVID infections seems to be amount of exposure too. So incorporating some type of time aspect into how long people are too close to each other could prove to be a better detector for new infections.

c. What limitations or improvements might you include in order to improve your proposed design?

It definitely takes some time to run the code, on my computer it took 7.5 minutes to process the 15 second rockstar video. If a program were to be analyzing live security footage, it would take much too long. Possibly analyzing every other frame or not every frame could improve the speed, because distance in between people isn't going to change much from frame to frame. 
