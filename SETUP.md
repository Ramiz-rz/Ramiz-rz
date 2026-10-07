# Setup (5 minutes)

1. On GitHub create a PUBLIC repo named exactly your username (e.g. `rameez-aslam/rameez-aslam`). Tick "Add a README".
2. Upload EVERYTHING from this folder (drag & drop works): all the .svg files (13 of them), README.md, `build/`, `profile-3d-contrib/` and `.github/` (hidden folder, make sure it uploads).
3. In README.md replace every `your-username` with your real GitHub username (Ctrl+F, replace all).
4. Repo -> Settings -> Actions -> General -> Workflow permissions -> "Read and write permissions" -> Save.
5. Actions tab -> run BOTH workflows once with "Run workflow":
   - "3D contribution city"  -> builds your 3D contribution city
   - "GitHub stats card"     -> fills the stats card with your real numbers
   Both then refresh daily by themselves.
6. Open github.com/YOUR_NAME to check it.

Optional: make the badge, project links and footer say your username too:
  cd build && pip install fonttools brotli && python3 build.py --user YOUR_NAME
(then upload the regenerated .svg files). Edit text in the CFG block at the top of build/build.py
and the project list in build/g_projects.py.
Art: build/art/ holds your images. Replace with --avatar / --figure, or swap the files.
