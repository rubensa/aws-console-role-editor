# "AWS Console Role Editor" extension for Google Chrome

This is a Google Chrome extension to manage roles from the Amazon Web Services (AWS) Console Cross Account delegation
(More about that [here](http://docs.aws.amazon.com/IAM/latest/UserGuide/walkthru_cross-account-with-roles.html)).

Currently this extension allows the following:
* Rename the display name
* Change account and role
* Modify the background color

### Installation
Clone the repository:

```bash
git clone git@github.com:rubensa/aws-console-role-editor.git
```

In Google Chrome, open the page [chrome://extensions/](chrome://extensions/)

Enable "**Developer mode**" in the top right.

Click "**Load unpacked**" button and select the cloned repository directory.

### Security
Because many people, including myself, are very sensitive using third party tools in AWS, you can check the code on your own.

#### Verify dependencies
To verify the dependencies, you can run:

```
wget -O- https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css | diff -s - css/bootstrap.min.css
wget -O- https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js | diff -s - js/bootstrap.min.js
wget -O- https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/fonts/glyphicons-halflings-regular.woff2 | diff -s - fonts/glyphicons-halflings-regular.woff2
wget -O- https://code.jquery.com/jquery-2.1.4.min.js | diff -s - js/jquery-2.1.4.min.js
wget -O- https://code.jquery.com/ui/1.12.1/jquery-ui.min.js | diff -s - js/jquery-ui.min.js
wget -O- https://raw.githubusercontent.com/bgrins/spectrum/1.8.0/spectrum.css | diff -s - css/spectrum.css
wget -O- https://raw.githubusercontent.com/bgrins/spectrum/1.8.0/spectrum.js | diff -s - js/spectrum.js
```

### Screenshots

![screenshot](images/screenshot.png "AWS Role Editor")
