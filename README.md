1. Extract the ZIP

Extract:

Fake_News_Detection-master.zip

For example, put the extracted folder on your Desktop:

cd ~/Desktop
cd Fake_News_Detection-master

Check the files:

ls

You should see files such as front.py, prediction.py, classifier.py, train.csv, etc.

2. Create a GitHub repository

On GitHub, create a new repository named:

Fake-News-Detection

Keep it empty — don't add README, .gitignore, or license yet.

3. Configure Git

Run these in Git Bash:

git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

Check:

git config --global --list
4. Initialize your project

Inside the project folder:

cd ~/Desktop/Fake_News_Detection-master

Then:

git init
git add .
git commit -m "Initial commit"
5. Connect it to GitHub

Replace YOUR_USERNAME with your GitHub username:

git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/Fake-News-Detection.git

Verify:

git remote -v
6. Upload the project
git push -u origin main

If GitHub asks you to authenticate, complete the GitHub sign-in/authentication process.

Then refresh your GitHub repository. Your project files should appear there.

▶️ Run the project locally

GitHub itself doesn't run the Python application. GitHub stores your code; you run the application on your computer (or deploy it to a hosting service).

First check Python:

python --version

Create a virtual environment:

python -m venv venv

Activate it in Git Bash:

source venv/Scripts/activate

Then install dependencies:

pip install pandas numpy scikit-learn nltk flask matplotlib seaborn

If your project has requirements.txt, use this instead:

pip install -r requirements.txt
Run the Flask website

From the project directory:

python front.py

You should get something similar to:

Running on http://127.0.0.1:5000/

Open this in your browser:

http://127.0.0.1:5000/
🔄 After making changes

Whenever you modify your code or README:

git add .
git commit -m "Update project"
git push

That's all you need.

⚠️ Important for your project

Because your ZIP contains trained model files and datasets, don't blindly use git add . if the repository becomes very large. First check:

du -sh .

and:

git status
