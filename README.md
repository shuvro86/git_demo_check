### Git Merge and Merge Conflict

```
echo 'Hello, World!' > code1.py
git init
git add code1.py
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/shuvro86/git_demo_check.git
git push -u origin main
```
```
echo 'Hello, World!' > code1.py
git add code1.py
git commit -m "Add initial code.py"
git push origin main
```
```
git checkout -b feature-1
```
```
echo 'Hello from Feature 11!' > code1.py
git add code1.py
git commit -m "Update code.py in feature-1"
git push origin feature-1
```
```
git checkout main
git checkout -b feature-2
```
```
echo 'Hello from Feature 2!' > code1.py
git add code1.py
git commit -m "Update code.py in feature-2"
git push origin feature-2
```


```
git checkout main
git merge feature-1
git push origin main
```
```
git checkout main
git merge feature-2
```

```
echo 'Hello from both features!' > code1.py
```


```
git add code1.py
git commit -m "Resolve merge conflict in code1.py"
git push origin main
```
