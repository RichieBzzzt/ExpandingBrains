# ExpandingBrains
Sample SSDT project to show options for referencing deployment scripts across composite projects.

It basically goes through the four different options that you have - no deployment scripts (Brain One), manually copying them over (Brain Two), editing the sqlproj file (Brain Three) or referencing the original scripts from the other scripts (Brain Four). Run the publishh.xml files and check the output for the messages being printed form the deplyoment scripts.

Clearly the best way with the least pitfalls is Brain Four. We can reference either particular scripts or the original post-deploy which will call all the others referenced by itself. Brain Three also allows us to do this, but stil lrequires editing sqlproj file, which puts off a lot of people. 
