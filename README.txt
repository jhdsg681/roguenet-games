RogueNet
========
This is a website made of several zip parts. Extract ALL the parts into the SAME folder
(say yes to merge/overwrite). You should end up with:
  index.html
  games/ covers/ hydra/ more/     (all included in the parts)
  play/                           (YOU add this one, see below)

play/ - copy the "games" folder from games-main.zip into here and rename it "play":
  robocopy C:\path\to\games-main\games C:\path\to\roguenet-site\play /E

Then upload the whole folder to GitHub and turn on GitHub Pages (Settings > Pages).
Use git from the command line - the website uploader can't take this many files.

broken-folders.txt lists folders inside play/ that are no longer used (broken or duplicate
games). To delete them and save space, open a terminal in the roguenet-site folder and run:
  for /f %i in (broken-folders.txt) do rmdir /s /q "play\%i"
