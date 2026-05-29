# Sample App to Manage your garden's plants!

# Installing using a Scratch Org

    1. Set up your enviroment. Follow the steps in the Quick Start: Lightning Web Components Trailhead project. The steps include:
        · Enable Dev Hub in your Trailhead Playground.
        · Install Salesforce CLI
        · Install Visual Studio Code
        · Install the Visual Studio Code Salesforce extensions, including the Lightning Web Components extension

    2. If you haven't already done so, authorize your hub org and provide it with an alias (myhuborg in the command below):
        · sfdx force:auth:web:login -d -a myhuborg

    3. Clone this repository:
        · git clone https://github.com/patriciaFiallos/plants26may26 cd plants

    4. Create a scratch org and provide it with an alias (plants in the command bellow):
        · sfdx force:org:create -s -f config/project-scratch-def.json -a plants

    5. Push the app to your scratch org:
        · sfdx force:source:push

    6. Assign the Plants_App permission set to the default user:
        · sfdx force:user:permset:assign -n Plants_App

    7. Import sample data:
        · sfdx force:data:tree:import -p ./data/data-plan.json

    8. Open the Scratch org:
        · sfdx force:org:open
