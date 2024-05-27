
# DD-Moneywash

## Description
A money laundering script for QB-Core in FiveM. This script allows players to launder money through a three-step process: washing, drying, and counting money, each with a separate location.

## Installation

1. **Download and Extract:**
   - Download the [DD-Moneywash.zip](sandbox:/mnt/data/DD-Moneywash.zip) file.
   - Extract the contents of the zip file to your `resources` directory in your FiveM server.

2. **Ensure Resource:**
   - Open your `server.cfg` file.
   - Add the following line to ensure the DD-Moneywash resource is started when the server starts:
     ```
     ensure DD-Moneywash
     ```

3. **Configuration:**
   - Open the `config.lua` file located in the `DD-Moneywash` folder.
   - Configure the percentage of black money to be laundered and the locations for each step of the laundering process.

     ```lua
     Config = {}

     -- Percentage of black money to launder (0-100)
     Config.LaunderPercentage = 85

     -- Locations for each step of the laundering process
     Config.Locations = {
         wash = {x = 1122.44, y = -3194.85, z = -40.4},
         dry = {x = 1132.44, y = -3194.85, z = -40.4},
         count = {x = 1142.44, y = -3194.85, z = -40.4}
     }
     ```

4. **Start Your Server:**
   - Start your FiveM server and the DD-Moneywash script will be loaded.

## Usage
- Players can launder their money by interacting with the defined locations for washing, drying, and counting money. Each step needs to be completed in sequence at its respective location.

## Support
- For any issues or support, please contact the script author or refer to the QB-Core documentation for additional help.
