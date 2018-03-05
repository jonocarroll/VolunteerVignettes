# VolunteerVignettes

The world needs more #rstats vignettes, so I'll be the change I want to see

# Automatic Conversion

One option is to convert existing `README.Rmd` files into vignettes; they typically contain a wealth of information which isn't actually contained within the package.

I've written a patch to the `usethis` package to allow for this; there are a few complications to navigate and I doubt I've correctly identified 100% of them. Nonetheless, it seems to do an okay job on some packages which have nice `README.md` files but no vignette: 

https://jonocarroll.github.io/VolunteerVignettes/fs/fs-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/mazealls/mazealls-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/patchwork/patchwork-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/remedy/remedy-README-vignette.html (large file size warning; lots of embedded gifs)
