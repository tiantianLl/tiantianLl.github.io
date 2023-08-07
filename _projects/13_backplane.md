---
name: Backplane
tools: [PCB Design, Signal Integrity, Mechanical Constraints]
image: /assets/backplane/spacing.png
description: Host the electrical system of AUV
---

# Backplane

The Backplane serves as the connection platform for all the custom electrical boards and the rest of the submarine. It is responsible for organizing and routing all of the interconnections between boards on the aft rack, as well as providing connectors for routing wires between the fore and aft racks of the sub.

Some of the design requirements includes:

- Facilitate all of the interconnections between boards on the aft rack in an organized manner, routing with proper trace widths to prevent any bottlenecks and electrical disturbances. TTL level is used on all the boards but it is susceptible to data loss in long or noisy wires. Therefore signals are converted to RS-232 level to be used on Backplane to reduce noise and corruption.

- Act as a liaison between aft rack boards and electronic components in the fore-rack of the sub, e.g., the sub’s forward-facing camera, main computer Jetson

- Provide an interface to SEACON-connected devices and components outside of the sub’s main hull, e.g., DVL, downward-facing camera, batteries, GX, hydrophone

- Comply with mechanical constraints such as dimensions, placement of screw holes, position of connectors for boards, clearance for wires, ease of access, heat dissipation

- Maintaining backward compatibility with old boards and be flexible to allow system extensions


![](/assets/backplane/sketch.jpg)
<p class="text-center">Designing Backplane</p>

![](/assets/backplane/power-signal.jpeg)
<p class="text-center">Power and Signal Considerations</p>

<div class="row">
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/3df.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/3db.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
</div>

<div class="row">
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/f.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/b.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
</div>

<p class="text-center">Final Product</p>


![](/assets/backplane/out-of-body.png)
<p class="text-center">Integration</p>


<div class="row">
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/racks-cad.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
    <div class="col">
        <img class="img-fluid" src="/assets/backplane/racks.png"
            onmouseover="" style="cursor: pointer;width:100%">
    </div>
</div>

<p class="text-center">Seamless integration with racks</p>


<img src="https://media.giphy.com/media/kJgZ0oiHcpGqonCKN1/giphy.gif" alt="racks of the sub" width="50%">
