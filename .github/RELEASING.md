# Releasing
The process to release this software looks a little different than with the original repository. Because GitHub workflows are involved, the process will automatically orchestrate the building of the SDL2 codebase, this codebase, merging the outputs of both into a NuGet package, and finally uploading that to NuGet.org for consumption.

The version used is directly tied to the SDL version in use.

1. Update the SDL_VERSION environment variable within the `publish.yml` file.
2. Push the changes to this repository (for a preview release build), or alternatively publishing a release.