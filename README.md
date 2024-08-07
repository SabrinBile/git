# Initialize a Git repository
git init
 
# Create a new file (e.g., main.py)
echo "print('Hello, World!')" > main.py
 
# Commit the initial version
git add main.py
git commit -m "Initial commit"
 
# Developer A adds a new feature
echo "print('Feature A')" >> main.py
git add main.py
git commit -m "Add Feature A"
 
# Developer B adds a different feature
echo "print('Feature B')" >> main.py
git add main.py
git commit -m "Add Feature B"
 
# Both developers push their changes
# Now the repository has concurrent changes
 
# Developer B pulls the latest changes
git pull origin master
 
# Developer A and B continue working...
