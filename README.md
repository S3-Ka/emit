# EMIT
Eve Online Marketing and Industry Tool

## Description
Standalone Python tool to help visualize blueprint costs and materials breakdown.

### What This Tool Is
* A pet project of mine.
* Provides general value breakdown of blueprints, compared to (Jita) market prices (using Janice)

### What This Tool Isn't
* Good. Or tested, even.
* A detailed profit margin planner.  Missing too many details: Build costs, taxes, etc.

### Why This Tool is Here
* To share my love of coding (read: hacking) with you
* To inspire you to make something better! (don't worry: the bar is really low :stuck_out_tongue:)

## Getting Started

### Installing

1. Install Python (I'm using 3.11.5)

2. Open Terminal (in my case PowerShell).
   * Change Directory (`cd`) to directory that has this stuff.
   * run: `python -m venv venv`
   * This creates a virtual python environment in a subdir named `venv`

3. Activate your virtual environment: `venv\Scripts\Activate.ps1` \
   (That's the PowerShell command.  If CMD, use the .bat version.)

4. Now install dependencies into your new virtual environment
   * First, upgrade pip: `python.exe -m pip install --upgrade pip`
   * Then use pip to install stuff into Python: `pip install flask requests pandas`

> [!TIP]
> Refer to requirements.txt to show exact versions that worked for me.\
> (Could use `pip install -r requirements.txt` to install my exact versions.)

### Customizing Configuration

(Optional, but Recommended)\
Get your own Janice API Key: https://github.com/E-351/janice?tab=readme-ov-file#api \
Replace the `X-ApiKey` in `market.py` header to match yours.\
(The key used currently is Janice's "public" key, from their examples)

## Executing Program

* Start the flask web server on localhost: `run.bat`
* Open your browser, point it to "http://127.0.0.1/"
* Click Builds, Add New Build. Type in an item you want to build.

## Acknowledgments
Special Thanks to Eve Online pilots Cat-Mix and Astral Destiny for their support in guiding and testing this tool.

### Supporting JS Projects
* Grid.js - MIT License: https://gridjs.io/docs/license 
* Chart.js - MIT License: https://github.com/chartjs/Chart.js/blob/master/LICENSE.md
* Go.js - Evaluation License: https://github.com/NorthwoodsSoftware/GoJS/blob/master/evaluationLicense.html
* jquery - MIT License: https://jquery.com/license/
* popper.js - MIT License
* bootstrap.js - MIT License: https://getbootstrap.com/docs/4.0/about/license/
* All Eve Online game data, fetched from https://www.fuzzwork.co.uk/dump/latest, derived from SDE, is owned by CCP Games
