PunctuationDumben (A Sigil Plugin)
============

"Dumben" smart punctuation in Sigil

A Sigil plugin wrapped for the SmartyPants software (Python based software to smarten punctuation, that includes a feature to remove such smartening).

This is forked from a plug-in that goes the other way (dumb to smart) and is useful for simplifying ePub books for older devices that don't properly render modern HTML entities.

**NOTE: this plugin periodically checks for updated versions by connecting to this Github repository**

Requirements
========

- Requires Sigil (tested on 1.9.2)
- Requires >= Python 3.4 (tested on 3.10.12)
- Requires Tkinter - see: [https://stackoverflow.com/a/74607246](https://stackoverflow.com/a/74607246)

Links
=====

* Sigil website is at http://sigil-ebook.com
* The SmartenPunctuation plugin support thread on Mobileread http://www.mobileread.com/forums/showthread.php?t=247088
* The Python SmartyPants software can be found at http://web.chad.org/projects/smartypants.py/
* The original "Smarten" plug-in that this is derived from: https://github.com/dougmassay/punctuationsmarten-sigil-plugin

Building
========

First, clone the repo and cd into it:

    $ git clone https://github.com/codepoet80/punctuationdumben-sigil-plugin.git
    $ cd ./punctuationdumben-sigil-plugin
    $ cd ..

To create the plugin zip file, run the buildplugin script (root of the repository tree) with Python (2 or 3)

    $ ./buildplugin

This will create the PunctuationDumben_vX.X.X.zip file that can then be installed into Sigil's plugin manager.

Contributing / Modifying
============
From here on out, a proficiency with developing / creating Sigil plugins is assumed.
If you need a crash-course, an introduction to creating Sigil plugins is available at
http://www.mobileread.com/forums/showthread.php?t=251452.


The core plugin files (this is where most contributors will spend their time) are:

    > newsmartypants.py
    > plugin.py
    > plugin.xml
    > utilities.py


Files used for building/maintaining the plugin:

    > buildplugin  -- this is used to build the plugin.
    > checkversion.xml -- used by automatic update checking (not yet implemented).
    > setup.cfg -- used for flake8 style checking. Use it to see if your code complies.

Feel free to fork the repository and submit pull requests (or just use it privately to experiment).



License Information
=======

### PunctuationDumben (a Sigil plugin)

    Licensed under the GPLv3.

### Based on [PunctuationSmarten (a Sigil plugin)](https://github.com/dougmassay/punctuationsmarten-sigil-plugin)

    Licensed under the GPLv3.

### SmartyPants (http://web.chad.org/projects/smartypants.py/)

    Copyright (c) 2003 John Gruber
    (http://daringfireball.net/)
    All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are
    met:

    *   Redistributions of source code must retain the above copyright
        notice, this list of conditions and the following disclaimer.

    *   Redistributions in binary form must reproduce the above copyright
        notice, this list of conditions and the following disclaimer in
        the documentation and/or other materials provided with the
        distribution.

    *   Neither the name "SmartyPants" nor the names of its contributors
        may be used to endorse or promote products derived from this
        software without specific prior written permission.

    This software is provided by the copyright holders and contributors "as
    is" and any express or implied warranties, including, but not limited
    to, the implied warranties of merchantability and fitness for a
    particular purpose are disclaimed. In no event shall the copyright 
    owner or contributors be liable for any direct, indirect, incidental,
    special, exemplary, or consequential damages (including, but not
    limited to, procurement of substitute goods or services; loss of use,
    data, or profits; or business interruption) however caused and on any
    theory of liability, whether in contract, strict liability, or tort
    (including negligence or otherwise) arising in any way out of the use
    of this software, even if advised of the possibility of such damage.
    smartypants.py license:

    smartypants.py is a derivative work of SmartyPants.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are
    met:

    *   Redistributions of source code must retain the above copyright
        notice, this list of conditions and the following disclaimer.

    *   Redistributions in binary form must reproduce the above copyright
        notice, this list of conditions and the following disclaimer in
        the documentation and/or other materials provided with the
        distribution.

    This software is provided by the copyright holders and contributors "as
    is" and any express or implied warranties, including, but not limited
    to, the implied warranties of merchantability and fitness for a
    particular purpose are disclaimed. In no event shall the copyright
    owner or contributors be liable for any direct, indirect, incidental,
    special, exemplary, or consequential damages (including, but not
    limited to, procurement of substitute goods or services; loss of use,
    data, or profits; or business interruption) however caused and on any
    theory of liability, whether in contract, strict liability, or tort
    (including negligence or otherwise) arising in any way out of the use
    of this software, even if advised of the possibility of such damage.
