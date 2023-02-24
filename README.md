LinUM1

Lab 9 - Package for distribution

A:
Modify electrotest to a standalone variant, i.e., electrotest-standalone.c

Create man-page
 
Create a deb-package to install electrotest-standalone

Delouse the package with lintian, excluding::
improbable-bug-number-in-closes
new-package-should-close-itp-bug

Extract information with command: dpkg-deb
Verify information with options -c -f

