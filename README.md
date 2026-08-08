# Mechatronics and Robotics Engineer

#### Technical Skills: CAD (Fusion 360), EasyEDA, VHDL, C++, MATLAB, Simulink

## Education
- MEng Mechatronics and Robotic Engineering | The University of Birmingham (_July 2026_)								       		

## Projects
### Robotic Waiter - Advanced Design Project

#### Overview

The Advanced Design Project is a University of Birmingham module where a team acts as a small-to-medium enterprise (SME) building a product for a client, under real commercial constraints: a £1,000 budget and a 3-month timeline. My team traded under the name **Caviar Tech Ltd.**, and our product was an autonomous robotic waiter.

I was voted team lead, responsible for organising the team and managing development.

![Robotic waiter chassis CAD](/assets/images/RoboticsWaiter/robotic-waiter-cad-full.png)
*Full chassis assembly in Fusion 360.*

#### My Role

Beyond running the team — assigning tasks by skillset, chairing weekly progress reviews against milestones — I worked hands-on in the physical build, across mechanical, electrical, and control systems. On the locomotion side, I started with BLDC motors running closed-loop PID, then moved the design over to stepper motors partway through development as the requirements became clearer.

![Motor mount CAD render]({{ "/assets/images/projects/robotic-waiter-teaser.png" | relative_url }})
*Custom motor mount design.*

#### What Actually Happened

The robot partially worked by presentation day — some parts failed shortly before we presented. The root cause wasn't any single subsystem: each part worked reasonably well on its own, but integration issues only surfaced once everything came together, and by then we were out of runway to fully resolve them. That's a time management lesson as much as a technical one — building in a dedicated integration-and-hardening phase well before the deadline, rather than treating integration as the last step, is what I'd change next time.

![Physical robot build in the workshop]({{ "/assets/images/projects/robotic-waiter-build.jpg" | relative_url }})
*The chassis mid-build in the workshop.*

#### What I Learned

- How to lead and coordinate a team of engineers under a hard deadline
- What running a project to a quality standard like **ISO 9001** actually demands in practice
- Why finished-product prototyping time needs to be protected earlier in a schedule, not squeezed in at the end

#### Skills Demonstrated

Team leadership · Motor control (closed-loop PID, stepper motors) · CAD design · Systems integration · Project & schedule management

### Field-Oriented Control for Railway Traction Systems

#### Overview

My final year research project investigated applying **Field-Oriented Control (FOC)** directly to the traction control loop of a railway locomotive, aiming to improve efficiency and handling over conventional control approaches. The project ran over 6 months and combined control-theory research with a physical prototype used to collect real test data.

![FOC railway locomotive prototype CAD]({{ "/assets/images/projects/foc-railway-teaser.png" | relative_url }})
*Prototype locomotive design — MOSFET driver board and traction motor mounted on a scale rail chassis.*

#### Why FOC on a Traction Loop

Traditional traction control on locomotives typically doesn't get the same precision benefits that FOC brings to smaller-scale brushless motor applications — treating the motor's torque- and flux-producing current components independently, rather than as a single combined quantity. Applying that same precision to a traction context was the core research question: does the efficiency and handling improvement FOC gives smaller BLDC systems carry over to a traction-scale loop, and what breaks when you try?

#### Building the Prototype

I designed and built a physical prototype to test the theory against real hardware rather than simulation alone — a scale locomotive chassis with a MOSFET driver stage, running on rail track, instrumented to collect performance data.

![FOC hardware prototype on breadboard]({{ "/assets/images/projects/foc-railway-prototype.jpg" | relative_url }})
*Early hardware iteration — motor driver board, gear-coupled BLDC motor, and breadboard control electronics.*

#### Outcome

The project scope was trimmed down from its original ambition to something deliverable in the time available, and FOC was successfully integrated into the traction loop — though with varying success across test conditions, largely driven by hardware limitations and sensor noise rather than the control algorithm itself. The work was well received by both my supervisor and the external examiner, and the resulting report is close to publishable quality with some further tightening.

#### What I Learned

- Practical implementation of advanced control algorithms, specifically FOC
- The fundamental working principles of three-phase brushless motors and how to precisely control them
- How to scope, execute, and write up an independent research project — including writing it to a standard that could plausibly be developed into a publishable paper

#### Skills Demonstrated

Field-Oriented Control · Three-phase BLDC motor control · Control system research & validation · Hardware prototyping · Technical writing

### Air Filtration Prototype — Healthcare in Conflict Zone

#### Overview

This was a large-scale engineering design module — around 40 students across multiple engineering disciplines, working in one team on a single brief: **healthcare in a conflict zone**. Our team's solution was a portable hospital, and as the Electrical and Mechatronic subgroup, we were responsible for the systems inside it. We chose an air purification unit as our physical prototype, built and tested on a £100 budget within a 3-month window.

![Finished air purification unit]({{ "/assets/images/projects/air-purifier-teaser.jpg" | relative_url }})
*The finished three-stage filtration unit — HEPA, activated carbon, and MERV filters, each independently removable.*

#### My Contribution

I worked on the intake CAD for the system and on the open-loop motor control that drives the fan.

![Air purifier CAD, exploded view]({{ "/assets/images/projects/air-purifier-cad.png" | relative_url }})
*Filter-stage CAD — removable HEPA, activated carbon, and MERV cartridges.*

#### System Design

Air passes through three filter stages in sequence, each targeting a different pollutant class:

- **HEPA** — particulates
- **Activated Carbon** — odours and VOCs
- **MERV** — a coarser pre-filter stage ahead of the two finer filters

A pair of onboard sensors feeds live readings back to a monitoring dashboard, tracking particulate concentration by size, mass concentration, VOCs, CO2, NO2, temperature, and humidity — giving a real Indoor Air Quality Index rather than a guess at filter performance.

![Live sensor dashboard readout]({{ "/assets/images/projects/air-purifier-sensor-data.jpg" | relative_url }})
*Live dashboard: particulate counts by size, VOC/CO2 estimates, and an Indoor Air Quality Index reading of 1 (clean air) after filtration.*

#### Testing

We tested the unit by sealing it inside a box and filling that box with smoke from incense sticks — a controlled, repeatable way to load the intake with particulates and VOCs without needing a real contamination source. The sensors detect the rise in VOCs and particulate count and drive the fan, and as the system runs, the dashboard shows air quality recovering back toward baseline in real time. All builds and tests were run to university health and safety standards.

#### Outcome

The prototype worked as intended — sensors detected the induced smoke, the fan responded, and air quality visibly recovered on the dashboard during testing.

#### What I Learned

- CAD skills for more complex, multi-part assemblies (removable filter cartridges, intake geometry)
- What it actually takes to build and test a working prototype inside real budget and time constraints, as one subgroup within a much larger team

#### Skills Demonstrated

CAD design · Open-loop motor control · Sensor integration · Air quality monitoring · Constraint-driven prototyping

### SIMAs - Eurobot

#### Overview

Eurobot is an international competition where teams build an autonomous robot to complete tasks that change every year. Alongside the main robot, teams also field smaller, simpler robots for the match called **SIMAs** (Small Independent Mobile Actuators). I worked mainly on the CAD for our SIMAs, making sure every design stayed within competition rules — on a 2-week timeline with no fixed budget.

![SIMA CAD design]({{ "/assets/images/projects/eurobot-sima-teaser.png" | relative_url }})
*SIMA design — compact drivetrain with onboard e-stop and control electronics.*

#### Design Constraints

The team set tight internal requirements on top of the competition rules:

- As simple as possible, both to design and to fix under time pressure
- Modular — parts had to be easy to swap if something failed close to competition day
- 3D-printable within 4 hours maximum per SIMA

#### Build

![Two SIMAs built and on the workbench]({{ "/assets/images/projects/eurobot-sima-build.jpg" | relative_url }})
*Two SIMAs on the workbench, showing the e-stop buttons and battery mounting.*

#### Outcome

The design met its own brief — it worked as intended, and was genuinely easy to interpret and modify when parts needed changing. Where it fell short was outside my scope: the final SIMA didn't get a full on-stage test at competition, due to coding issues elsewhere on the team. A reminder that a mechanically sound design still depends on everything else around it being ready too.

#### What I Learned

Designing within genuinely tight constraints set by the team itself, not just the competition rulebook — and finding solutions that satisfy both at once.

#### Skills Demonstrated

CAD design for manufacturability · Rapid prototyping (sub-4-hour print budgets) · Modular mechanical design · Competition robotics

### Custom Keyboard PCB

#### Overview

A personal project, built for a genuinely personal reason: I use multi-key shortcuts often enough that some of them are hard to remember reliably. Rather than keep fumbling for combinations, I designed a custom macro keyboard PCB around an ESP32 - and used the project as a chance to properly learn hotplate SMD assembly.

#### Design & Assembly

I designed the board in EasyEDA, then assembled it by hand using a hotplate and solder paste rather than sending it out for assembly - a reflow process that leaves very little margin for error on paste placement and temperature control with fine-pitch components.

#### Debugging

The first boards didn't work. I ran into shorts from paste bridging during reflow, and the harder problem to trace, the USB data lines weren't sending the correct sequence to initialize communication with the ESP32, so the board wasn't enumerating over USB at all. I went through each board's failure mode one at a time, checking for bridged pads, then working back through the USB D+/D- lines until I had a board that enumerated and worked as intended.

#### What I Learned

- Hotplate reflow and solder paste assembly, hands-on
- How to debug hardware systematically when a board doesn't come up separating "this pad is bridged" from "this is a signal integrity/protocol problem," which look identical from the outside but need completely different fixes

#### Skills Demonstrated

PCB design (EasyEDA) · Schematic capture · Reflow soldering · Systematic hardware debugging · ESP32 / USB enumeration

## Other projects
- Birmingham Tech Week - University Elevate Program
- UBRobotics Drones workshops
- Forged Carbon Fibre Workshops
- Glove controlled rover robot
- Matlab simulation on Green Hydrogen production plant
- IMeche Design Challenge
- Tool Sanitisation station - Health Care in Conflict Zone
- UBRacing - Formula Student team member

