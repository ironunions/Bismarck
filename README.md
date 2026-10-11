# Bismarck

**Bismarck** is a lightweight, asynchronous private server emulator for [Azur Lane](https://en.wikipedia.org/wiki/Azur_Lane), built with Python 3.12+ and `asyncio`. Designed specifically for the official EN Android release, it allows players to connect using a completely unmodified, stock game client. 

This repository is a fork of [PrivateDock](https://github.com/Forlorn01/PrivateDock), which itself evolved from [Belfast](https://github.com/ggmolly/belfast).

---

## AI & Development Disclaimer

Like PrivateDock before it, Bismarck's codebase incorporates AI assistance (ChatGPT) during development. While software engineering isn't my primary background, I actively test features, resolve issues, and strive to keep the emulator as stable as possible. 

Unforeseen bugs or edge cases may still pop up during gameplay—if you encounter any errors or unexpected behavior, please feel free to open an issue or share feedback!

---

## Feature Overview

Bismarck provides functional support for a wide range of Azur Lane's primary gameplay mechanics.

### Included Systems
* **Base & Interface**: Secretary configurations and Juustagram.
* **Fleet Management**: Dockyard, fleet setups (including submarine units), gear/equipment, and Meowfficers.
* **Ship Acquisition**: Construction (featuring custom maximum order caps and customizable build pools, allowing you to pull for ships outside the live server rotation—such as collab events or Priority Research ships), Requisition, and Retirement.
* **Progression & Facilities**: Shops, Missions, Handbook, Tactical Classes, Dormitory, Fleet Tech, Research Academy, and Shipyard.
* **Combat & Game Modes**: Main Story Campaign, War Archives, Daily Raids, and Exercises.

> For a complete feature list, partial implementation details, and upcoming goals, review the **[Implementation Status](docs/STATUS.md)** guide.

---

## Quick Start Guide

> **Note**: Step-by-step setup details and prerequisites are available in the **[Installation Documentation](docs/INSTALL.md)**.

1. **Prerequisites**
   * Python 3.12+ installed on your system.
   * An official Azur Lane EN client.
   * The [AzurLaneLuaScripts](https://github.com/AzurLaneTools/AzurLaneLuaScripts) repository.

2. **Clone Repositories & Set Up Environment**
   ```bash
   git clone [https://github.com/AzurLaneTools/AzurLaneLuaScripts.git](https://github.com/AzurLaneTools/AzurLaneLuaScripts.git)
   git clone [https://github.com/YOUR_USERNAME/Bismarck.git](https://github.com/YOUR_USERNAME/Bismarck.git)
   cd Bismarck

   python -m venv .venv

   # Activate virtual environment
   # On Windows (PowerShell):
   .venv\Scripts\Activate.ps1
   # On Linux / macOS:
   source .venv/bin/activate

   pip install -r requirements.txt
