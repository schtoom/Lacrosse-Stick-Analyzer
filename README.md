# Lacrosse-Stick-Analyzer

The goal of this project is to create a device capable of identifying different, specific motions/activities with a lacrosse stick.  To start, we'll just work with identifying a standard upright pass.

There are three phases of this project.

Phase 1 - Create a collector of information.  This is a backpack that contains a sensor package to collect motion/position information.  There is a button to initiate recording (a 1.5s recording of 150 samples from each sensor).  Each button press creates a new file on the microSD card - the file can be ejected and the data on the card can be used to analyze movements.  Since we're planning on using a machine learning algorithm for classification purposes, we'll want to collect different types of motions as data.

Phase 2 - Create and tune a machine learning classification algorithm to identify a standard upright throw to start.

Phase 3 - Create a backpack for a lacrosse stick using the same sensor package that is capable of either running the ML algorithm locally or transmitting the data from the packge to another device.  The goal is to collect the data in real time and run the ML algorithm ever 1/4 second or so and provide instant feedback if a movement was detected.
