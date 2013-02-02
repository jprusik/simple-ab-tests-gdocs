Simple A/B Tests with Google Docs
=================================

Purpose
-------
Simple A/B Tests with Google Docs is a lightweight technique for quick, basic, and straightforward A/B testing of HTML elements. By utilizing HTML event parameters along with JavaScript, simple testing of click-through rates, load rates, and/or user changes can be achieved.

Usage
-----
You can find a working example [here](http://jprusik.github.com/simple-ab-tests-gdocs/index.html).

You'll need to create a new Google Doc form with two text fields. Grab the form key from the "published form link".

Make sure your form is public (the corresponding spreadsheet does not need to be public).

Call `clickTrack()` when and where you want to test the second event (by default, the first event is recorded after the test element to be displayed is determined).

Don't forget to update or remove `<noscript>` contents.

Limitations/Known Issues
------------------------

This specific implementation has a Google Docs dependency.

Page loads are anonymous (No location data recorded).

No IP filtering or any other de-duplication techniques are utilized.

Default configuration assumes a desired 50/50 split between the 'A Test' and 'B Test'.

The `<input>` id and name parameters assume a default Google Docs form. If you create/delete/recreate fields on your form, you will need to update the id and name parameters to reflect the change in fields.

Author
-------
Jonathan Prusik @jprusik [www.classynemesis.com]