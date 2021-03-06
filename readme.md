Ex Libris Student Portal Sample App - My Rails Library
================================================

Introduction
------------

This is a port of the [My Alma Library sample application](https://github.com/jweisman/MyAlmaLibrary) into Ruby on Rails.

The original application does the following:
* Authentication with Google OAuth
* Library card- displays some basic student information and allow users to update a few key data elements
* Requests- shows a list of the student's requests, and allow the user to cancel them

More information about the original C# app is available in this [blog entry](https://developers.exlibrisgroup.com/blog/Creating-a-Student-Portal-with-the-New-Alma-APIs).

About the App
-------------
The application is written in Ruby on Rails and uses the new Alma APIs described [here](https://developers.exlibrisgroup.com/alma/apis). As with all demo applications, we include the following disclaimer: in an effort to increase readability and clarity, only minimal error handling has been added.

Installation Instructions
-------------------------
On any machine with [Ruby on Rails](http://rubyonrails.org/) and [Git](http://git-scm.com/) installed, do the following:

1. Clone this repository: `git clone https://github.com/jweisman/my-alma-rails-library.git`
2. Install dependencies: `bundle install`
3. Copy the `application.example.yml` file to `application.yml` and replace the placeholder values:
  * `almaurl` from the [Alma API Getting Started Guide](https://developers.exlibrisgroup.com/alma/apis)
  * `apikey` from the [Ex Libris Developer Network](https://developers.exlibrisgroup.com/) dashboard
  * `googleclientid` and `googleclientsecret` from the [Google Developer Console](https://console.developers.google.com/)
4. Run the application: `bin\rails server` for WEBrick or `bundle exec puma` for Puma

