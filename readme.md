#### Remove noise by stacking images and finding median
`convert $(ls) -evaluate-sequence median out.jpg`

#### Resize all images in a folder
`for f in *.jpg; do convert "$f" -resize 2000x2000 "small/$f"; done`
