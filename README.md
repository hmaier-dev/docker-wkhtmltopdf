# Image
Build the image with the `+build`-target and the fitting version tag:
```bash
earthly +build --tag="v1"
```
If you want to push the image to the Github Container Registry, use the `--push`-flag.
```bash
earthly +build --tag="v1" --push
```
