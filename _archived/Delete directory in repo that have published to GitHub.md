--- 
tags: GitHub
---

I have uploaded projects in which some folders that need to be ignored are not added to the `.gitignore` file, resulting in uploading some files that I didn't want to upload. (for example, accidentally uploading the `_site` to repo:`kitamado.github.io`)

- solution
```bash
git rm -r --cached _site  #--cached won't delete _site localy
git commit -m 'delete _site_ dir'
git push -u origin main
```
