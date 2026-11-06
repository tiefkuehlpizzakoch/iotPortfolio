# Module 1
> **Example module** from the IoT introduction class. Adjust the headings and tasks to match your actual course content.

> When you start editing this file, remove this description.
>
> Usually the first things you have to document are some inspirations hinting at what
> you might be able to build in this class, a personal profile description regarding
> programming expertise, previous MCU knowledge, creative qualities, and expectations

Module description

## Learning Goals

> **How to use the learning goals.** Copy the module's learning goals from the course workbook into the block below. Keep the `LG1`, `LG2`, … IDs and a one-word keyword. In each task, write `Proves: LG2` (or link to `[LG2](#lg2)`) so you can find the evidence quickly at checkpoint time. In the **Evidence** line under each goal, link to the task that proves it.

<a id="lg1"></a>
### LG1 — `<keyword>`

Explain how this class works — learning goals as the contract, negotiable tasks, evidence in a portfolio — and start your own portfolio with a note on what you already know, what you expect, and who your pod is.

**Evidence:** [Task Inspirations](#task-inspirations)

<a id="lg2"></a>
### LG2 — `<keyword>`

Explain publish/subscribe with an MQTT broker: the star topology, hierarchical topics, wildcards, and why decoupling producers from consumers is what makes an IoT system maintainable.

**Evidence:** [Task Personal Profile](#task-personal-profile)

<a id="lg3"></a>
### LG3 — `<keyword>`

Build Node-RED flows that subscribe and publish, turn a physical button into a remote actuator action, and render live telemetry as a gauge, a chart, and a wildcard aggregation.

**Evidence:** [Task What is IoT](#task-what-is-iot)

<a id="lg4"></a>
### LG4 — `<keyword>`

Wire a digital 1-wire sensor, read its value over MQTT, and explain the declarative OTA loop (one line in setup.cpp → a fleet-wide deployment) and what it changes for a real fleet.

**Evidence:** [Task Personal Profile](#task-personal-profile)

<a id="lg5"></a>
### LG5 — `<keyword>`

Critically analyze the ISO/OSI 7-layer model against real TCP/IP in IoT systems (referencing RFC 3439 and RFC 1958), and quantify header overhead from a capture taken at the edge — the router, an ESP32 tap, or a provided dump — stating every assumption.

**Evidence:** [Task Personal Profile](#task-personal-profile)

<a id="lg6"></a>
### LG6 — `<keyword>`

Craft a system story that is concrete enough to pitch, spanning the computing continuum with named stakeholders, devices, and interfaces — and name the weakest link in it.

**Evidence:** [Task Personal Profile](#task-personal-profile)

<a id="task-inspirations"></a>

## Who am I?
Programming experience: Python, Java, C(++)
Never used a microcontroller.
Never configured a router.
Never used Wireshark.
I have used MQTT, the command line and Git / GitHub before.
I'd like to connect sensors like moisture sensors with a Dashboard.
I expect to get the hands-on experience I need for my own home automation projects.

## Study log
Task 1:
<a href="https://github.com/Rein2Max/iot-test/blob/main/Module01/README.md"></a>
Task 2:
Based on our discussions, the TCP/IP model simplifies the OSI Model by aggregating Session, Presentation and Application Layers into ONE common Application Layer, while Data Link and Physical Layers belong to Network Access Layer.

Task 3: Screenshot is in: ./pictures/

Task 4: the button and LED are on the same board, but the signal took a round trip through the network because the firmware publishes the button press to the broker and subscribes to a separate topic for the LED, so the board talks to the broker, not directly to itself.

Task 5: it allows for asynchronous communication and decouples message producers from consumers, enhancing scalability and flexibility in distributed systems. Its single point of failure typically lies in the message broker, which can disrupt message delivery if it fails; to mitigate this, implementing redundancy or failover mechanisms for the broker would be beneficial.

Task 6: the cable is needless because the data was transfered to the stick, allowing the stick to work with the data afterwards

Task7: If each pod had invented its own topic names, the wildcard subscription (`+/temp`) would break, making it impossible to aggregate all sensor data from the room into a single, unified chart or heatmap.

## Task Inspirations

**Proves:** [LG1](#lg1)

- Inspiration 1
- Inspiration 2

<a id="task-personal-profile"></a>
## Task Personal Profile

**Proves:** [LG2](#lg2)

<a id="task-what-is-iot"></a>
## Task What is IoT

**Proves:** [LG3](#lg3)

Domains and included areas:

-
-

Commonly used (data) protocols:

-
-

Typical devices (appliance or micro controller):

-
-

Challenges:

-
-

## Reflection 1

[Reflection 1](../Reflections/ref01.md)
