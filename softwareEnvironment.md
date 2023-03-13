# Software
Some useful software / tools to work with OpenFOAM.

## Text editor, IDE and overall command center
Visual Studio Code (or short VS Code) is the best solution for all needs in terms of text editing and preparation of simulations. Extremely flexible also through the add-ins. Advantages are (not a complete list):
- tabbed editor
- nice search-and-replace function also over multiple files
- Can be a full IDE through extensions 
- Remote management through SSH plugin
- GIt integration
- Debugging tools
- syntax highlighting
- Workspaces (open multiple directories at once)
- Extensive theming and customization options

## SSH Tools
To access remote machines (such as a cluster or a local high performance machine), SSH will be useful.

### MobaXTerm
For an integrated beginner-friendly solution, MobaXTerm is great. File management, multiple terminal tabs, X-Window support. Free versions available (and also a portable version, so no installation required)
https://mobaxterm.mobatek.net/

### Windows Terminal
Windows terminal is a Microsoft product (free), which has tabbed terminal tabs. SSH does not require Putty or something like that anymore, but can be executed directly from a powershell window

### Putty
Not really required anymore, as Powershell supports the SSH command.

### WinSCP
Utility to transfer files. Might be useful in some cases, but files can also be transfered through SSH with VS Code or directly from powershell with `scp`.


## Preprocessing
### BricsCAD
UFZ has some ancient AutoCAD license. But BricsCAD (essentially an AutoCAD clone) has a free academic license. Runs also on Linux!

### OpenSCAD
For parametric STL generation

### GUI options for blockMesh etc.
THere are several options to have a graphical interface for blockMesh or snappyHexMesh. There are add-ins for Blender and FreeCAD, processing toolboxes such as the HELYX-Toolbox, IHfoam, simscale and many more. Helyx and IHfoam might be useful to get started, but in the end it's more efficient to work with "normal" textfiles (and without those GUI helpers) - especially when working on a cluster later on.

### Other Meshing Options
GMSH is used by many. Works well for many cases. CFmesh is shipped with OpenFOAM [PDF introduction](:/b44a121c6d6a4134a4f681ce19a03138), and can be useful for some cases.
The Salome-Platform is another option for meshing, especially when going for triangles / prismatic meshes.

### 2D-Meshing
For direct 2D-Meshing the only option in OpenFOAM is blockMesh. Snappy is 3D, but can be tricked into a 3D-Mesh by using extrudeMesh.
Other options for 2D-meshing are gmsh or the salome-toolbox.


### PyFOAM
pyFoam is a python add-on for OpenFOAM. There are countless utilities. Some are working well, some not so much. There are utilities to quickly create multiple case variations, clean up cases etc. 

For checking the case at runtime, the pyFoamPlotWatcher (in conjunction with foamRun) is useful. (needs x-window output though, so either x-forwarding or to execute through a virtual desktop environment).


## PostProcessing
### Paraview
First and foremost... Create the `a.foam` file in the simulation directory to open the results in Paraview. 

### Python / PyFOAM / onboard tools
For number output, the easiest way is oftentimes to use postProcessing output directly from OpenFOAM (generated through function objects), or generated with pyFOAM. Further processing with python, e.g. in a jupyter notebook.
Works quite well. For advanced processing, pvpython can be useful (paraview python). Get some help on generating paraview python scripts by using the macro recorder in the Paraview GUI.

## Notes
### Joplin
FOSS markdown notes app. Can be connected to Nextcloud (through Nextcloud or WebDAV) to have a backed up / synced notetaking app environment.
With all the markdown advantages (such as support of math, code blocks, quick and easy formatting, file attachments, interoperability)
Customization possible through addins / plugins
Available for all platforms (incl. mobile)
https://joplinapp.org/

### Notion
A VERY powerful option. Maybe a bit too powerful? ;)

### Evernote
a commercial alternative to Joplin, but quite limited in the free tier

### OneNote
Doesn't really support math and code blocks in a nice way

## Citations
### Zotero
The only option which supports all relevant operating systems (Win, Mac, Linux, iOS, Android).
Supported also by most scientific tools such as SciFlow or Overleaf.
Can be connected to a private cloud through WebDAV + Zotero Account -> full "cloud" citation manager for free
Very nice iOS app (for reading and annotating papers on a tablet)
Collaboration is possible through that cloud solution.

### Citavi
Not recommended. Very weak multi-platform approach - only a web-version which took >8 years to develop. 

### EndNote
Commercial. Might be good if you have a license?

### Mendeley
Not tested.


