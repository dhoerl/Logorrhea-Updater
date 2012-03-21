Q: What is Logorrhea?
A: A Mac OS X program used to search and browse your iChat repository (ie your old iChats)

Q: What is this updater?
A: The two files in this repository are a shell program and patch file that downloads the original 1.3.1 Logarrhea source from Spiny.com, and applies a patch file to it to create a more modern version with bug fixes.

Q: Why the patch file? Why don't you distribute the updated source.
A: Read the Logarrhea licence (Logorrhea Read Me.rtf). People may download and use the code for their own use, but are not allowed to redistribute it.

Q: Why won't Spiny give you permission to distribute fixes as long as you maintain their copyright?
A: No idea?

Q: Why don't they roll your bug fixes into their code?
A: No idea. I have tried for around to 5 years now to get them to take my fixes, for a while they chatted, but in the last year the line has gone dead. Meanwhile, I alone have been using bug free code to probe my iChat respository.

Q: So, if I run your patch script on my computer, can I then redistribute the source or binary?
A: Well, read their license ((Logorrhea Read Me.rtf). I personally do not believe you can legally do either.

Q: Why shouldn't I just use their original binary?
A: Well, it does still work. A few bugs prevent it from seeing all text in all chats, so you find yourself failing to find some bit of information that you know is in some chat (this is how I found some bugs!) Also, when you build the original source you will get many "Deprecated" warnings, so at some point the original code will just not work anymore. The updated code builds without any warnings.

In addition to a few bug fixes, the updated source:

- properly parses the new iChat "GroupChat" object, making that text searchable.
- uses ARC and the 64 bit runtime
- opens to the search pane not the browse pane
- builds with no warnings


HOW TO CREATE THE UPDATED SOURCE:

- in Terminal, run the attached shell file "patcher" (you can read it first to see what it does)
- if xcodebuild is installed, it runs it otherwise opens the project in Xcode.

