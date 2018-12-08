Introduction Bower

Web sites are made of lots of things — frameworks, libraries, assets, and utilities. Bower manages all these things for you.

Keeping track of all these packages and making sure they are up to date (or set to the specific versions you need) is tricky. Bower to the rescue!

Bower can manage components that contain HTML, CSS, JavaScript, fonts or even image files. Bower doesn’t concatenate or minify code or do anything else - it just installs the right versions of the packages you need and their dependencies.

To get started, Bower works by fetching and installing packages from all over, taking care of hunting, finding, downloading, and saving the stuff you’re looking for. Bower keeps track of these packages in a manifest file, bower.json. How you use packages is up to you. Bower provides hooks to facilitate using packages in your tools and workflows.
Bower is optimized for the front-end. If multiple packages depend on a package - jQuery for example - Bower will download jQuery just once. This is known as a flat dependency graph and it helps reduce page load.

Install Bower
Bower is a command line utility. Install it with npm.

npm install -g bower

Bower requires node, npm and git.

Latest release: bower version

For troubleshooting installation on different platforms, read the troubleshooting wiki page.

Getting started
Install packages
Install packages with bower install. Bower installs packages to bower_components/.

bower install <package>
A package can be a GitHub shorthand, a Git endpoint, a URL, and more. Read more about bower install.

- installs the project dependencies listed in bower.json
bower install
- registered package
bower install jquery
- GitHub shorthand
bower install desandro/masonry
- Git endpoint
bower install git://github.com/user/package.git
- URL
bower install http://example.com/script.js
Search packages
Search Bower packages and find the registered package names for your favorite projects.

Save packages
Create a bower.json file for your package with bower init.

Then save new dependencies to your bower.json with bower install PACKAGE --save

- Use packages
How you use packages is up to you. We recommend you use Bower together with Grunt, RequireJS, Yeoman, and lots of other tools or build your own workflow with the API. You can also use the installed packages directly, like this, in the case of jquery:

<script src="bower_components/jquery/dist/jquery.min.js">
</script>
