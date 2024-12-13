# Plot MOs

## generate cube
### Multiwfn
```
gencube.sh xxx.fch "range of orb" prefix
```
### PySCF

## render
run vmd
```
vcube xxx*cub
vstyle white-red
viso 0.02 -0.02
display resize 600 600
display resetview
```

## convert figures
```
bmp2png.sh prefix xscale yscale
magick montage prefix*c.png big.png
```
options for montage
```
-tile x1 # layouts
```

# Plot moles
```
vmol xxx.cub
```
tricks
```
fog
display cueend 3.5
```