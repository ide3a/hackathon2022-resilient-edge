# ide3a Hackathon 2022: Resilient Edge Challenge

The internet of things (IoT) and edge computing are core components of future smart cities. Interconnected computing systems will perform tasks beyond measuring and monitoring, and will also make decisions and take over highly critical tasks. Especially in disaster situations, such as extreme weather events, where for e.g. traffic control can be crucial to guarantee safety, we should therefore not rely on grid power supply to be available at all times. 

In this challenge, we deal with an edge node in a smart city which receives and executes offloading jobs from connected vehicles (e.g. compute-heavy tasks that would otherwise drain the vehicle’s batteries). However, during power outages the edge node is only powered by a solar panel, so there is not always enough energy to compute all offloading requests.

Based on this scenario, students will investigate strategies to maximize the usefulness of an edge node under emergency conditions. For this, they will first need to clarify the assumptions for their concrete use case (do we have a battery or solar production forecasts? Do requests have different priorities or urgencies?) and then define the goal of their approach (e.g. maximize the number of requests under certain risk constraints). Solutions to this challenge can either be concrete approaches evaluated via a simulation, or you can develop conceptual ideas and analyze/visualize data to support them.

Resources:
- [Cucumber: Renewable-Aware Admission Control for Delay-Tolerant Cloud and Edge Workloads](https://arxiv.org/pdf/2205.02895.pdf). Philipp Wiesner, Dominik Scheinert, Thorsten Wittkopp, Lauritz Thamsen, and Odej Kao. Euro-Par. 2022.
- [SimPy](https://simpy.readthedocs.io): Python discrete-event simulation framework
- [LEAF](https://github.com/dos-group/leaf): Simulator for modeling energy consumption in edge computing based on SimPy
- [Mosaik](https://mosaik.offis.de/): Co-Simulation engine for electric grids + whatever else you want to simulate


## Installation

Download this repository using either `git` or simply clicking `Code` -> `Download ZIP` on the GitHub website.

Within the repository directory, we now install the requirements for running the simulation in Jupyter lab:

```
python3 -m venv venv              # create venv
. venv/bin/activate               # activate venv
pip3 install -r requirements.txt  # install dependencies
```
For Windows:
```
.\venv\Scripts\activate           # activate venv
```
You can now start Jupyter lab by running `jupyter lab`, which should open a new browser window/tab. 
Open `main.ipynb` and sequentially run all cells.

If all the notebook cells run without errors, you are ready to attend the practical session!
