WHAT IS TiAir?
===========================
TiAir is an MVC framework for Appcelerator Titanium Mobile.

It's really an MVCN framework, which is something I have made up on my own to address the unique differences from a typical
MVC framework designed for the web and a mobile implementation of it. You can guess already that "MVC" stands for "Model
View Controller". The "N" stands for "Navigator". This crucial component is responsible for deciding how to handle "URLs"
that your app requests. For example, opening a URL in a tab, or expanding a modal pop up from a specific point on the screen.


HOW DO I USE IT?
===========================
To use its features, include the TiAir.js file at the top of your app.js, and initialize it.

For now, check out the jab11 repository to see TiAir in action.

https://github.com/rblalock/jab11

<pre>
Ti.include('TiAir.js');
TiAir.init({

    // the default URL is the entry point for the app; after everything is initialized, we'll open this URL
    // note that it is a controller-action pair with as many optional arguments as you want. We'll magically map any
    // objects you pass here into their matching arguments on the specified controller's action.
    defaultURL: { controller: 'default', action: 'list' },

    // your controllers decide who is going to do stuff, and what they are going to do it with
    controllers: [
        'default.js'
    ],

    // models contain data
    models: [
        'defaultIcons.js'
    ],

    // navigators control the transitions between views in your app
    navigator: 'default.js',

    // views show something to the user; a single view can contain other views, and usually receives a model
    views: {
        shared: [
            'button.js'
        ],
        'default': [
            'daysUntil.js', 'list.js'
        ]
    }
});
</pre>

You will then need to create (or copy from an existing TiAir project) the folder structure common to an MVC project.
Check out the jab11 project to see how each model, view, and controller is set up and can interact.

https://github.com/rblalock/jab11


WHAT THE FUTURE HOLDS
===========================
	1) We will be creating samples of how to use TiAir.
	2) Lots of easy to use shared views with examples of their use. For example, a table with cross platform pull to refresh.
    3) More examples of navigators for different usage scenarios. Tabs, menus, navigator groups, settings, etc.


CONTACT INFORMATION
===========================

Redux was made by Dawson Toth and Rick Blaloc from Appcelerator, Inc.

Note that this doesn't mean TiAir is officially supported.
If you have issues, PLEASE open an issue on GitHub and we will work on getting it resolved!
Don't contact Appcelerator with issues, or sue them (or me, please) if you have problems.