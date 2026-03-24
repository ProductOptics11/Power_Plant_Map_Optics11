Split-file web map package for GitHub web upload

Why this version exists
- GitHub browser uploads are limited to 25 MiB per file.
- This package splits the GeoJSON into 3 smaller files so you can upload through the GitHub website.

Files
- index.html
- data_part_1.geojson
- data_part_2.geojson
- data_part_3.geojson
- .nojekyll

Steps
1. Create a new GitHub repository.
2. Upload all files in this folder to the root of the repository using the web UI.
3. In the repo, go to Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Choose your main branch and the /(root) folder.
6. Open the published site URL.

Notes
- Keep all files in the same folder.
- The map will load the three GeoJSON parts automatically.
- If you replace the data later, keep the same filenames or update the list in index.html.
