#### Remove noise (or people) by stacking images and finding median
`convert $(ls) -evaluate-sequence median out.jpg`

#### Resize all images in a folder
`mkdir -p small && ffor f in *.jpg; do convert "$f" -resize 2000x2000> "small/$f"; done`

#### Auto level
`convert t.png -auto-level out.jpg`

#### Auto level and resize
`mkdir -p small && for f in *.jpg; do convert "$f" -resize 2000x2000> -auto-level "small/$f"; done`
