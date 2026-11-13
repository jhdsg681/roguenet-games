RogueNet - complete package (10 zip parts)
=========================================
The site is split into 9 zips: roguenet-part1.zip ... roguenet-part10.zip.
Extract ALL 10 into the SAME empty folder (say yes to merge). You will see:
  index.html   .nojekyll   README.txt
  wallpapers/  icons2/  ck/  games/  hydra/  more/  play/
Nothing else is needed.

Put the whole folder online with git (the website uploader cannot take this many files):
  cd path\to\this\folder
  git init
  git branch -M main
  git remote add origin https://github.com/YOURNAME/YOURREPO.git
  git add index.html .nojekyll README.txt wallpapers icons2 ck games
  git commit -m "site"
  git push -u origin main --force
  git add more
  git commit -m "more"
  git push
  git add hydra
  git commit -m "hydra"
  git push
  git add play
  git commit -m "play"
  git push
Then turn on Settings > Pages > main branch > root folder in the repo.
If a push fails, run the same "git push" again.

In the site: Settings > Check games finds games that no longer load and can hide them.
Settings > Game saves lets you export a backup of your saves.
