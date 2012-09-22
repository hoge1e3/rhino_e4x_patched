This program is rhino1_7R2 with following modifications:

* Fix the bug on parsing E4X literal (ex. var x=<a>{bar(<b/>)}</a> );
-- see https://bugzilla.mozilla.org/show_bug.cgi?id=323890
* Modify java.mozilla.javascript.ScriptRuntime::escapeString not to escape UTF8 wide characters.

This program is used to make rhino_patched.jar in soyText( https://github.com/hoge1e3/soyText ).
rhino_patched.jar is created by Eclipse -> export -> jar file

== Modified files/directories from rhino1_7R2.zip

* These directories are removed:
 deprecatedsrc examples javadoc testsrc toolsrc
* all files in the top level directory are removed except LICENSE.txt
* moved and overrwrite xmlimplsrc/org to src/org
* added .project and .classpath (Eclipse project file) and README.txt(this file)

* These file are modified:

 src/org/mozilla/javascript/Parser.java
    modified at 2011/11/26
 src/org/mozilla/javascript/ScriptRuntime.java
    modified at 2011/11/27
 src/org/mozilla/javascript/TokenStream.java
    modified at 2011/11/26

 All Modified lines have following string:
hoge1e3


== License

This program is MPL 1.1 / GPL 2.0 dual licensed.

== Contact

hoge1e3[ a t ]gmail.com

