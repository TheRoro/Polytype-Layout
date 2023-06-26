# Linux Installation

## Instructions

In order to install the **Polytype Layout** in a Linux Distribution, you should follow the next steps:

1. Navigate to the following route in your computer:

```
/usr/share/X11/xkb/symbols
```

2. Copy the [Polytype](https://github.com/TheRoro/Polytype-Layout/blob/main/downloads/linux/polytype) file in this location. You may be prompted to provide root access in order to save it.

![Linux Ubuntu - Symbols Folder](https://raw.githubusercontent.com/TheRoro/Polytype-Layout/main/downloads/linux/images/symbols_folder.png "Linux Ubuntu - Symbols Folder")

3. Open the `/usr/share/X11/xkb/rules/evdev.xml` file and add the following information:

```xml
<layout>
  <configItem>
    <name> polytype </name>
    <shortDescription> Polytype Layout </shortDescription>
    <description> Polytype Layout </description>
    <languageList>
      <iso639Id> eng </iso639Id>
    </languageList>
  </configItem>
  <variantList/>
</layout>
```

Make sure to insert it as the **last entry** within the `<layoutList>` element. Save the file.

![Linux Ubuntu - evdev.xml file](https://raw.githubusercontent.com/TheRoro/Polytype-Layout/main/downloads/linux/images/evdev_xml.png "Linux Ubuntu - evdev.xml file")

4. Locate the `/usr/share/X11/xkb/rules/xorg.lst` file. In this file, find the section labeled "**! layout**" and **add the name of the layout**, "Polytype Layout," at the end.

![Linux Ubuntu - xorg.lst file](https://raw.githubusercontent.com/TheRoro/Polytype-Layout/main/downloads/linux/images/xorg_lst.png "Linux Ubuntu - xorg.lst file")

5. Navigate to `Settings -> Region & Language` on your computer. Under the "**Input Sources**" section, click the "+" button and search for "Polytype Layout." Select it from the list of options.

![Linux Ubuntu - Layout List Selection](https://raw.githubusercontent.com/TheRoro/Polytype-Layout/main/downloads/linux/images/list_selection.png "Linux Ubuntu - Layout List Selection")

Now, you should see the Polytype Layout option in the **upper-right corner** of your screen, allowing you to switch to it.
