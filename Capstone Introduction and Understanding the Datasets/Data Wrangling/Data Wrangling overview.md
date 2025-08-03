# Data Wrangling Review

In this project, we will review **data wrangling**.

We will work with several attributes from the dataset:

* **Flight Number**
* **Date**
* **Booster version**
* **Payload mass**
* **Orbit**
* **Launch Site**
* **Outcome**: this is the status of the first stage
* **Flights**
* **Grid Fins**: these help with landing
* **Reused**
* **Legs**: used in landing
* **Landing pad**
* **Block**
* **Reused count**
* **Serial**
* **Longitude and latitude of launch**

### Launch Sites

The column `LaunchSite` contains different launch locations, including:

* Vandenberg AFB Space Launch
* Kennedy Space Center
* CCAFS SLC 40

### Orbits

The column `Orbit` shows the different orbits of the payload. For example:

* **LEO**: Low Earth orbit is an Earth-centered orbit with an altitude of 2,000 km.
* **GTO**: A geosynchronous orbit is a high Earth orbit that allows satellites to match Earth's rotation. It is located at 22,236 miles (35,786 kilometers) above Earth's equator.

### Outcomes

The column `Outcome` indicates whether the first stage successfully landed. There are 8 types. For example:

* **True ASDS**: the booster successfully landed on a drone ship.
* **False ASDS**: the mission outcome was unsuccessful and the booster did not land on the drone ship.

We aim to convert landing outcomes into **classes `y`** (either `0` or `1`):

* `0` is a **bad outcome**: the booster did not land.
* `1` is a **good outcome**: the booster did land.

The variable **`Y`** will represent the **classification variable** for the outcome of each launch.