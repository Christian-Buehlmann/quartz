[[ReadItLater]] [[Article]]

# [Retrieve annotations for Hypothes.is via Templater plugin (Hypothes.idian)](https://forum.obsidian.md/t/retrieve-annotations-for-hypothes-is-via-templater-plugin-hypothes-idian/17225/4)

I use [https://hypothes.is/](https://hypothes.is/) to annotate web sites and web based pdf’s. I want to easily import them into Obsidian. This script uses the Templater template.

Template File: [Templater script hosted on GIST GitHub](https://gist.github.com/tfthacker/c48bca69f1520deed0ecbc8840f6241a)

Script in action:

[![](https://forum.obsidian.md/uploads/default/original/2X/f/fc541344d06dae1c926ade9d6e3ebef93d245404.jpeg "hypothes.idian Demo  for Obsidian")](https://www.youtube.com/watch?v=f-mVj_DSaag)

It is ready for testing. Feedback welcome.

27 Likes

I’ve never used the Templater Plugin, But can you tell me how to achieve what you are doing in the video.

I’ve done the following;

1.  Made the Hypothesis config.md file with only my token inside, it’s in my vault.
2.  I’ve made a note in my templates folder named Hypothesis, basically it is the note where I copy pasted the GIST you provided
3.  I’ve edited the gist to have my token where it’s written UserToken and my Hypothes.is account name where it says UserId.

**Now I just want to achieve what you are doing in the video. What additional steps are required? Or am I missing some basic Keyboard shortcuts.**

1 Like

I’m very interested in this as well, however I’ve never had occasion to work with Gists. Would you be willing to more specifically explain what to do with the code and files?

I tried the same thing as [@Daniyal-Ahmed](https://forum.obsidian.md/u/daniyal-ahmed) with no success. I suspect I need to “run” the gist somehow. Thanks in advance!

Install steps:

1.  Install Templater plugin in Obsidian
2.  Configure your templates folder in the templater settings page in “settings”
3.  Copy the text in the gist to a file in your templates folder for templater
4.  Now you can run that script (press ALT+E) and select the script you copied in.
5.  The first time it runs, it creates they Hyposthesis config.md file for you with all the settings you need.

After that run the script and select the command you want.

2 Likes

Please see my other post to this thread with install steps. GIST is just a way to store files on the web and share them. Go to the gist page in the link, click on the “RAW” button, which shows you all the text you need and copy that a file in the templater templates folder.

1 Like

I didn’t realize using the template would “activate” the code. That’s what I needed to get it working. I obviously haven’t tested much yet but if I find issues, I’ll let you know.

This is absolutely fantastic. Thanks so much for sharing!

my pleasure. sorry i am new to templater as well. It is running the code in the file. lots happening there ![:slight_smile:](https://forum.obsidian.md/images/emoji/apple/slight_smile.png?v=9 ":slight_smile:")

Ok, That’s How it’s done. Thank You [@TfTHacker](https://forum.obsidian.md/u/TfTHacker), for writing this script. It is very useful to annotate while you are reading something on the web and then Export it into Obsidian later. This way we don’t need to move back and forth from Obsidian and Browser to write notes.

1 Like

This is a great Templater script. Thanks, [@TfTHacker](https://forum.obsidian.md/u/TfTHacker).

1 Like

Hey peeps, fixed a bug today that the config file generated by this script can be stored any where in your graph, not just in the root folder.

1 Like

Great addition. I can’t say having it in root was *bad*, but it’s nice to tuck it away.

Thanks again for the script. I plan to wean myself off Zotero for those times when I don’t need a full blown reference.

1 Like

I’ve modified a portion of the template to better suit my own use. I’ve posted [a Gist of my version](https://gist.github.com/chrisaldrich/031c946446b1bc070b1937f330989c63) for those who’d prefer it or would like an alternate example of an modification of the template section. Perhaps it may help those who are not as code-savvy puzzle out how they might make their own modifications?

The changes still keep all the relevant data fields, but reorder them and add a bit of formatting to fit the layout and the way I use my Obsidian notebook. In particular, I changed the formatting so that tags in Hypothes.is are turned into \[\[wikilinks\]\] rather than #⁠hashtags as in the original. (The original also doesn’t do so well with multi-word tags in Hypothes.is, which I use quite a lot.)

3 Likes

This is amazing. I didn’t know about Hypothes.is, despite having tried a few of its “competitors”. I’m looking forward to playing with it and to have such an easy link to Obsidian will almost certainly make this my “go to” tool. Thank you for your efforts.

The only issue I’ve found with this plugin is if I have annotations on a local PDF file (using Chrome and the Chrome Hypothes.is extension). It crashes. Remove any local PDF annotations and it works again. I’ve not been able to parse the JSON from Hypothes.is yet to see what is fundamentally different.

Not a biggie for me - I generally host PDFs on the cloud - but just thought I’d mention.

Edit: Main difference seems to be the URI/Source which is a fingerprint of the local PDF: e.g. “uri”: “urn:x-pdf:a999faa94eb5eb4efefee1f1e1b519482”

[nat](https://forum.obsidian.md/u/nat) July 28, 2021, 2:49pm #14

This is beyond amazing! Thank you so much.

1 Like

This is a great process. It would be good to include the step by step in your post and/or in the video. As a newbie to Obsidian and Mark Down, these help my note processing go much faster. Just wanted to say thank you!

1 Like

Hi David, I wanted to ask what cloud solutions one can use to achieve something like getting a raw PDF display in the browser. I am using OneDrive, but I don’t think it redirects you to / give you a raw pdf link in any way. Thanks in advance

[Wen](https://forum.obsidian.md/u/Wen) October 22, 2021, 7:34pm #18

[pupka12](https://forum.obsidian.md/u/pupka12) December 19, 2021, 5:33pm #19

Does anyone know a way to do this with my annotations on locally stored pdfs? That would be lovely.  
I know I could probably move them to some cloud, but I have no idea which one could work (the most popular ones seem not to)

[Wen](https://forum.obsidian.md/u/Wen) December 20, 2021, 6:30pm #20

If you use Zotero, the following workflow may be of interest:

If you are on the macOS, PDF readers like PDF Expert can also extract highlights as Markdown:

If you are on the macOS and uses [Alfred - Productivity App for macOS](https://www.alfredapp.com/), the following workflow can also extract annotations:

3 Likes