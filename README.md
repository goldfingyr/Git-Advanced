# Git-Advanced
**Når GitHub-Desktop ikke er nok...**

Disse situationer dækkes ikke i undervisningen, men det forhindrer dem ikke i at opstå!

Som alle andre in-app git-tools har også Github-Desktop sine begrænsninger.
Her finder du så mulige løsninger på situationer som ellers synes uløselige.

Vær opmærksom på at disse løsninger inkluderer CLI (Command Line Interface) anvendelse af Git og også andre Git tools.

## Repository migration
[Video link](./docs/LostRemoteRepo.mp4)
* **Hvordan flytter jeg mit git fra et GitWorld system til et andet GitWorld system**
* **Vore gruppe splittede og jeg vil lave en kopi af projekt-repository som jeg har skriverettighed til**

**Procedure:**
* Create an empty repository on your chosen GitWorld
* Create an application key authorized to write repositories
* `git remote remove origin`
* `remote add origin URL_AND_APL_KEY_TO_DST_GITWORLD_REPO`
* `git push origin main`

## Merge Conflict
[Video link](./docs/MergeConflict.mp4)
* **Github-Desktop kan ikke løse min merge conflict**
* **Jeg vil gerne have et bedre visuelt merge conflict værktøj**

**Tools used:**
* [WinMerge](https://winmerge.org/)
* [Git for Windows](https://gitforwindows.org/)
* [Git Extensions](https://gitextensions.github.io/)

**Procedure:**

## Retrospekt aktivering af .gitigore
[Video link](./docs/LostRemoteRepo.mp4)
* **Jeg glemte .gitignore så nu er der mange binære filer i repositoriet**
* **Jeg har ændret .gitignore men der er stadig gamle uønskede filer**

**Procedure:**
* Commit og push alle ændringer. Ellers risikerer du at miste de ændringer, du har foretaget
* **git rm -r --cached .**  << Husk punktum til sidst!
* **git add .**  << Husk punktum til sidst!
* **git commit -m ".gitignore is now working"**
