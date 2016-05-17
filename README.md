# TiPasscode
iOS passcode input view

Optimized for iPhone and iPad. Should word on Android too.

~~~
// Init the passcode view
var passCodeControl = require('/lib/passcode');
var passcodeView = new passCodeControl();

// true, if you want the user to enter the code to save it within the app
// false, if you want to ask for the saved code
passcodeView.setPromptMode(true);

// Display the view
passcodeView.display();

// Eventlistener
passcodeView.addEventListener('passcode.success', function (e) {
	console.log(e.passcode);
});

passcodeView.addEventListener('passcode.cancel', function (e) {

});

passcodeView.addEventListener('passcode.close', function (e) {
	console.log(e.passcode);
});
~~~
