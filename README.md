#### Project for generating static websites using jekyll on OSX High Sierra 

##### Use atom for webdev [atom](https://atom.io)
> Install the following packages: 
- vim-mode-plus 
- enmet
- atom-live-server 


> Check to make sure you have ruby and jekyll installed. 
```bash
ruby -v			# check if ruby is installed, if not:
brew install ruby

jekyll -v		# check if jekyll is installed, if not: 
sudo gem install jekyll
```

> If installing for the first time, you will need to install the  necessary jekyll dependancies. See detailed instructions [here](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/).

> Use below instructions to install jekyll + dependencies. 
```bash
cd /[yoursite]/templates	# change to your site dir

vim Gemfile			# create a new Gemfile or modify existing one 

# add to Gemfile 

source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins

# save and exit 

bundle install			# install jekyll and dependencies  

# fork, clone a template jekyll site to your [yoursite]/templates dir

git clone [forked-repo] 

cd [forked-repo]

bundle exec jekyll serve	# run jekyll site locally; check http://localhost:4000 

```
