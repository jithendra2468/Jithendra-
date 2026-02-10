

# Step 1: Create README.md file
echo "Name: Your Name" > README.md
echo "College: Your College Name" >> README.md
echo "Workshop Date: 10-02-2026" >> README.md

# Step 2: Initial Commit
git add README.md
git commit -m "Initial commit"
git push origin main

# Step 3: Create New Branch
git checkout -b intro-branch

# Step 4: Create intro.txt file
echo "Name: Your Name" > intro.txt
echo "Department: Your Department" >> intro.txt
echo "One Hobby: Reading" >> intro.txt

# Step 5: Commit intro.txt
git add intro.txt
git commit -m "Added intro.txt file"
git push origin intro-branch

# Step 6: Merge into main branch
git checkout main
git pull origin main
git merge intro-branch
git push origin main

# Step 8: Delete intro-branch
git branch -d intro-branch
git push origin --delete intro-branch
