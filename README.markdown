railify
=======
Utility script which generates a rails app with an initialized git repo and installs some standard gems/plugins.

Features
------------
 - Generates an Edge Rails App
 - Initializes a git repo with the standard `.gitignore` for rails development
 - Creates mysql databases with `rake db:create:all`
 - Copies Edge into `vendor/rails`
 - Installs and sets up `rspec, haml, and resource_controller`

Forked
------
New Features / Changes
 - No longer uses braid
 - Git no longer ignores application.css (does not assume that sass is being used to generate it)
 - Uses FileUtils for mass removal of unnecessary files
 - Clears logs instead of removing them
 - Uses config.gem to add gems

Usage
-----
    railify new_app_name

