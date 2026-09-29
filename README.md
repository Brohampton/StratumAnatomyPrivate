# Stratum Anatomy

Interactive 3D human anatomy atlas. Static site: no server code, no build step.

## Files that must be in your repository

    index.html
    .nojekyll
    models/manifest.json
    models/skin.bin.gz
    models/fascia.bin.gz
    models/muscles_superficial.bin.gz
    models/muscles_deep.bin.gz
    models/organs.bin.gz
    models/cns.bin.gz
    models/lymph.bin.gz
    models/arteries.bin.gz
    models/veins.bin.gz
    models/nerves.bin.gz
    models/ligaments.bin.gz
    models/skeleton.bin.gz
    models/LICENSE-models.txt

index.html and the models folder must sit side by side in the repository root.
File and folder names are case-sensitive: keep "models" lowercase and do not rename anything.

## Test locally (optional)

Opening index.html by double-click will NOT load the models (browsers block file:// fetches).
Run a tiny local server in this folder instead:

    python3 -m http.server 8000

then open http://localhost:8000

Credits and licences for the 3D data are in models/LICENSE-models.txt and in the site footer.
