# Amoskeag KiCAD libraries

## Add to your project

To add into your project

```
git submodule add https://github.com/Amoskeag/Amoskeag_KiCAD_Libs
```

## 3D Models

open `Preferences` and `Configure Paths` then add the following enviorment variable:

```
Name: AMOSKEAG_3DMODELS
Path: <Path to folder>
```


## Kibot

And if you use kibot, add this to your `pre_flight`

```
preflight:
  ...
  set_text_variables:
    - name: "AMOSKEAG_3DMODELS" # 3D models for Amoskeag Library
      command: "echo 'Hardware/Board/Libraries/Amoskeag_KiCAD_Libs/3D'"
```

# Projects using this lib:

https://github.com/Amoskeag/RoboDojo

https://github.com/Amoskeag/Balance-Bot