Completed Chapter1!:

Some errors/warnings on my way:

(*) warning: Insecure world writable dir /Users in PATH, mode 040777
http://stackoverflow.com/questions/2796421/warning-insecure-world-writable-dir-when-i-run-a-ruby-or-gem-command

The obvious work-around is to remove "other" write permission from the relevant directories:
 
chmod o-w /path/to/dir

(*)problems with ssh keys not in /.ssh | was using /Users/....

tested my connection with:
$ ssh git@github.com

$ ssh -v git@github.com. 

This will print out debug info on what ssh is trying to do. 
In this output you should check that ssh is connecting to the correct server, 
on the correct port (22). 
Many firewalls and proxies will block this connection. 
Also ensure that ssh is reading the correct key files, 
these are at ~/.ssh/id_rsa, id_dsa and identity by default. 
If your key is not at this location, you should move it or create an override 
(see the “SSH config” section below).

(*)
/Users/tatic/.rvm/rubies/ruby-1.9.2-p136/lib/ruby/1.9.1/rubygems.rb:762:in `report_activate_error': 
Could not find RubyGem heroku (>= 0) (Gem::LoadError)

heroku keys:add /.ssh/id_rsa.pub

cat ~/.ssh/id_rsa.pub | pbcopy


bundle install

git remote add origin git@github.com:user/app.git

git push origin master

git checkout -b modify-README (Create branch and checkout)

gem install heroku

heroku create

# push the app to Heroku
git push heroku master

Tatiana-Carvalhos-MacBook:first_app tatic$ bundle show heroku
/Users/tatic/.rvm/gems/ruby-1.9.2-p136@rails3tutorial/gems/heroku-1.17.10

heroku open
Opening http://app.heroku.com/

heroku rename your_new_name

ruby generate a random name
('a'..'z').to_a.shuffle[0..7].join








