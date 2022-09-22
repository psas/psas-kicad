# psas-kicad
Repo for KiCAD libraries and footprints and such.

## Getting started

To start using these libraries, you should set up an environment variable within KiCAD pointing to `psas-kicad` on your system.

* In the KiCAD menu open Preferences > Configure Paths.
* Under "Environment Variables" click the "+" button to add a new environment variable and name it `PSAS_LIBRARIES`.
* In the path area, enter (or browse for) the `psas-kicad` repository on your system.
* Click Ok.

That's it! Now when you open a project that uses these libraries with the `PSAS_LIBRARIES` variable, KiCAD will use the path you provided to locate them.

## Adding libraries to your project

Once you've set up the `PSAS_LIBRARIES` environment variable, you can also start adding these libraries to your own projects.

* Open up your project.
* In the project panel, choose Preferences > Manage Symbol Libraries.
* Select the "Project Specific Libraries" tab.
   * MAKE SURE YOU ADD THE LIBRARY TO "Project Specific Libraries" AND NOT "Global Libraries".
* Click on the Folder icon below.
   * THIS IS IMPORTANT. DO NOT CLICK ON "+". CLICK ON THE FOLDER.
* In your project folder, navigate to `psas-kicad/psas-symbols` and choose the symbol(s) you want. You can include all of them if you want!
* Choose Open, then OK.
* Back in the project panel, choose Preferences > Manage Footprint Libraries.
* Select the "Project Specific Libraries" tab.
   * MAKE SURE YOU ADD THE LIBRARY TO "Project Specific Libraries" AND NOT "Global Libraries".
* Click on the Folder icon below.
   * THIS IS IMPORTANT. DO NOT CLICK ON "+". CLICK ON THE FOLDER.
* In your project folder, navigate to `psas-kicad/psas-footprints` and choose the footprint libraries you want.
* Choose Open, then OK.

At this point, your project should be pointing to your psas-kicad repository and you should be good to go!
