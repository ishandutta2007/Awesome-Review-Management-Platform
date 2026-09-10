# Awesome-Review-Management-Platform

# This has to be run from C:\Users\ishan\Documents\Projects folder

$repo_name = 'Awesome-Review-Management-Platform'

$repo_desc = 'Top Review Management Platform (Opensource) 🌟 Star if you like it! 🌟'



$loops_path="C:\Users\ishan\Desktop\Coding_LOOPs"

if (-not $env:GITHUB_TOKEN) { Write-Error "Error: set GITHUB_TOKEN in enviroment first"; Start-Sleep -Seconds 30; exit 1 }

$GITHUB_TOKEN=$env:GITHUB_TOKEN

if (-not $env:loops_path) { Write-Error "Error: set loops_path in enviroment first"; Start-Sleep -Seconds 30; exit 1 }

$loops_path=$env:loops_path

create-github-repo $repo_name -d $repo_desc --token $GITHUB_TOKEN

mkdir $repo_name

cd $repo_name

echo "# $repo_name" >> README.md

echo "" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin "https://github.com/ishandutta2007/$repo_name.git"

git pull origin main --allow-unrelated-histories

git push -u origin main



git add .

git commit -m "first code"

git push



# add-github-topic applied-ai --token $GITHUB_TOKEN

gh repo edit ishandutta2007/$repo_name --add-topic "curated-list,awesome-list"

git pull



github-tabs Discussions --token $GITHUB_TOKEN

git pull



github-tabs Sponsorships --token $GITHUB_TOKEN

git pull



github-protect --token $GITHUB_TOKEN

git pull



git add README.md

git commit -m "first code"

git pull

git push



cp ..\Awesome-BERT\.gitignore .

git add .\.gitignore

git commit -m .\.gitignore



cp ..\Awesome-BERT\LICENSE .

git add .\LICENSE

git commit -m .\LICENSE



git rm --cached *.bak

git status

git add .

git commit -m cleanup



git push

gh browse



$real_repo_name=$repo_name.replace('Awesome-','')

chatgpt-cli "$loops_path\sheet_outputs\$real_repo_name.txt" -o "../$repo_name/README.md" -w 600

# grok-cli "$loops_path\sheet_outputs\$real_repo_name.txt" -o "../$repo_name/README.md" -w 600

# -b chrome

(Get-Content -Path "../$repo_name/README.md") -replace "## Top ", "### Top " | Set-Content -Path "../$repo_name/README.md"

# subl .

git add .

git commit -m minor_title

git push



github-growth-plot --publish

git add .

git commit -m growth_plot_added

git push



gh-browse-or-reload 





git config --global --add safe.directory '*'

git fsck

if (Test-Path .git/index.lock) { Remove-Item .git/index.lock -Recurse -Force }



agy --dangerously-skip-permissions --sandbox
