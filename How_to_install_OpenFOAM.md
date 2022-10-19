## How to install from OpenFOAM.com: [Guide video](https://www.youtube.com/watch?v=CeEJS1eT9NE) 

## Fix error: The repo is not longer signed (OpenFOAM.com)
### Edit the corresponding line in /etc/apt/sources.list : 
deb [arch=amd64 trusted=yes] https://dl.openfoam.com/repos/deb bionic main
([Source:](https://www.cfd-online.com/Forums/openfoam-installation/243709-repo-not-longer-signed-openfoam-com.html))

## How to install ParaView: [Guide video](https://www.youtube.com/watch?v=tWEGjWD8d2M)

```bash
sudo gedit ~/.bashrc
```
- Type this code line in .bashrc file: 
```
export PATH=$PATH:/opt/ParaView-5.9/bin
```

```bash
sudo ln -s /opt/ParaView-5.8/bin/paraview /usr/bin/paraview
sudo ln -s /opt/ParaView-5.8/lib/paraview-5.8/ /usr/bin/paraview-5.8
```

```bash
sudo gedit /usr/share/applications/paraview.desktop
```
- Type this code lines in paraview.desktop file:
```
[Desktop Entry]
Version=1.0
Name=Paraview 5.8
Exec=paraview
Terminal=false
Icon=/opt/ParaView-5.8/share/icons/hicolor/96x96/apps/paraview.png
Type=Application
x-Ayatana-Desktop-Shortcuts=NewWindow
[NewWindow Shortcut Group]
Name=New Window
Exec=paraview
TargetEnvironment=Unity
```
