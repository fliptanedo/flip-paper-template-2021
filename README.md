# flip-paper-template 2021
A LaTeX paper template that I use for papers and notes. [GitHub Location](https://github.com/fliptanedo/flip-paper-template-2021); replaces [older version](https://github.com/fliptanedo/flip-paper-template).

By Flip Tanedo (flip.tanedo@ucr.edu)

Uses Jacques Distler's `utcaps.bst` and AAS TeX's `aas_macros.sty`, included in this repository. Place figures in the `\figures` directory. 

## How to use this

For those, like me, are less competent with `git` and GitHub than we really aught to be.

1. Go to repo's [page](https://github.com/fliptanedo/flip-paper-template-2021) on GitHub.

2. Click on the green `Code` button just to the top-right of the list of files. 

3. Copy the URL that pops up. It should be:
   `https://github.com/fliptanedo/flip-paper-template.git`

4. Locally (on your system) go to the parent directory of where you'd like to start a new LaTeX project and open a Terminal (command prompt) window there. Assuming you have `git` set up, you can simply type in

   ```
   git clone https://github.com/fliptanedo/flip-paper-template.git 
   ```

5. and press enter.

6. This should create a new folder `flip-paper-template`. Go ahead and rename it right away:

   ```
   mv flip-paper-template new-folder-name
   ```

7. Go ahead and start your new project.

8. If you'd like to put this new project on GitHub:

   1. Start a new GitHub repository through the web interface. 

   2. Do **not** initialize with a `README.md` file. 

   3. Follow the steps to push an existing repository.  **Except**: there's one problem. Your copy of `flip-paper-template` (now renamed) is *already* connected to the paper template GitHub repository. This should be:

      ```
      git remote set-url origin [https://github.com/....git]
      git push -u origin master
      ```

      Where the first line is changed from `git remote add origin`. Note that `master` [may be renamed](https://www.git-tower.com/learn/git/faq/git-rename-master-to-main/) to `main`.

   4. [Alternately](https://stackoverflow.com/questions/17546246/git-cloning-repository-into-new-repository) (in place of previous step), you can remove the obsolete remote and then add the new remote:

      ```
      git remote rm origin
      git remote add origin [https://github.com/....git]
      ```

      

That should do it.