# Step 1: Clone Repository
git clone https://github.com/jithendra2468/github-workshop-assessment.git
cd github-workshop-assessment

# Step 2: Create README.md file
echo "Name: DEVIREDDY JITHENDRA REDDY" > README.md
echo "College: KALASALIGAM UNIVERSITY" >> README.md
echo "Workshop Date: 10-02-2026" >> README.md

# Step 3: Initial Commit
git add README.md
git commit -m "Initial commit"
git push origin main

# Step 4: Create New Branch
git checkout -b intro-branch

# Step 5: Create intro.txt file
echo "Name: DEVIREDDY JITHENDRA REDDY" > intro.txt
echo "Department: CSE" >> intro.txt
echo "One Hobby: Reading books" >> intro.txt

# Step 6: Commit intro.txt
git add intro.txt
git commit -m "Added intro.txt file"
git push origin intro-branch

# Step 7: Merge into main branch
git checkout main
git pull origin main
git merge intro-branch
git push origin main

# Step 8: Delete intro-branch
git branch -d intro-branch
git push origin --delete intro-branch
