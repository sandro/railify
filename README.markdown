railify
=======
Utility script which generates a rails app with an initialized git repo and some standard gems/plugins installed.

Features
------------
 - Generates an Edge Rails App
 - Initializes a git repo with the standard `.gitignore` for rails development
 - Creates your databases with `rake db:create:all`
 - Copies Edge into `vendor/rails`
 - Installs, unpacks, and sets up `rspec, haml, and annotate_models`

Forked
------
New Features / Changes
 - No longer uses braid
 - Git no longer ignores application.css (does not assume that sass is being used to generate it)
 - Uses FileUtils for mass removal of unnecessary files
 - Clears logs instead of removing them
 - Uses config.gem to add and unpack gems

Usage
-----
    railify rails_app

