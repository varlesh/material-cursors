# Windows Implementation

### How to Build from X Cursor Set


### Deps

1. Download and Install http://www.rw-designer.com/cursor-maker

2. Download and Install Gimp (or whatever Photoshop software you like)

### How to Generate Cursor file

1. Open .svg file from `src/{theme}/{file}.svg` in Gimp

2. Export the .svg as .png

3. Open .png in RealWorld Cursor Editor

4. Edit as you like

5. Save as .cur file (Windows-format cursor file)

6. Edit the `Install.inf` file to add or edit whatever your file you changed:

```
...
[Scheme.Cur]
"Arrow.cur"
"Help.cur"
"AppStarting.ani"
"Wait.ani"
"Cross.cur"       
"IBeam.cur"
"Handwriting.cur"
"NO.cur"
"SizeNS.cur"
"SizeWE.cur"
"SizeNWSE.cur"
"SizeNESW.cur"
"SizeAll.cur"
"UpArrow.cur"
"Hand.cur"


[Strings]
CUR_DIR         = "Cursors\Materia Light"
SCHEME_NAME     = "Materia Light"
pointer		= "Arrow.cur"
help		= "Help.cur"
work		= "AppStarting.ani"
busy		= "Wait.ani"
cross		= "Cross.cur"
text		= "IBeam.cur"
hand		= "Handwriting.cur"
unavailiable	= "NO.cur"
vert		= "SizeNS.cur"   
horz		= "SizeWE.cur"
dgn1		= "SizeNWSE.cur"
dgn2		= "SizeNESW.cur"
move		= "SizeAll.cur"
alternate	= "UpArrow.cur"
link		= "Hand.cur"
...
```

7. Right-click, install, click "yes" when asked if you want to overwrite existing cursor set. 