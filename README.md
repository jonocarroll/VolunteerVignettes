# VolunteerVignettes

The world needs more #rstats vignettes, so I'll be the change I want to see

# Automatic Conversion

One option is to convert existing `README.Rmd` files into vignettes; they typically contain a wealth of information which isn't actually contained within the package.

I've written a patch to the `usethis` package to allow for this; there are a few complications to navigate and I doubt I've correctly identified 100% of them. Nonetheless, it seems to do an okay job on some packages which have nice `README.md` files but no vignette: 

https://jonocarroll.github.io/VolunteerVignettes/fs/fs-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/mazealls/mazealls-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/patchwork/patchwork-README-vignette.html

https://jonocarroll.github.io/VolunteerVignettes/remedy/remedy-README-vignette.html (large file size warning; lots of embedded gifs)

Performing these conversions highlighted some issues with the process, even after careful treatment; mainly images in unexpected (to the vignette) places. But it also highlighted some neat issues with the READMEs themselves; packages used in the `README` which weren't marked as `Import`/`Suggests`, and image locations not existing. In theory more could be wrong; there is nothing stopping the `README` from becomming stale. Vignettes are built on install, so something should get flagged either on local check/build/install or during continuous integration testing.