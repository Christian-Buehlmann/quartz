[[ReadItLater]] [[Article]]

# [Git and Version Control for Novelists, Screenwriters, Academics, and the General Public](https://boffosocko.com/2014/09/17/revision-control/)

## Marginalia and Revision Control

At the end of April, I read an article entitled “[In the Margins](http://krieger.jhu.edu/magazine/v11n1/in-the-margins/ "In the Margins | Johns Hopkins University Arts & Sciences Magazine")” in the Johns Hopkins University Arts & Sciences magazine.  I was particularly struck by the comments of eminent scholar [Jacques Neefs](http://grll.jhu.edu/directory/jacques-neefs/ "Jacques Neefs") on page thirteen (or paragraph 20) about computers making marginalia a thing of the past:

> Neefs believes contemporary literature is losing a valuable component in an age when technology often precludes and trumps the need to save manuscripts or rough drafts. But it is not something that keeps him up at night. ‘The modern technique of computers and everything makes \[marginalia\] a thing of the past,’ he says. ‘There’s a new way of creation. Some would say it’s tragic, but something new has been invented. I don’t consider it tragic. There are still great writers who write and continue to have a way to keep the process.’

![Photo looking over the shoulder of Jacques Neefs onto the paper he's been studing on the table in front of him.](https://i0.wp.com/boffosocko.com/wp-content/uploads/2014/04/Neefs.jpg?fit=342%2C359&ssl=1)

Jacques Neefs (Image courtesy of Johns Hopkins University)

I actually think that he may be completely wrong and that current technology actually allows us to keep far more marginalia! (Has anyone heard of [*digital exhaust*](http://www.deloitte.com/view/en_US/us/Services/additional-services/deloitte-analytics-service/short-takes/d1c68e6b7b407310VgnVCM1000001956f00aRCRD.htm "digital exhaust")?) The bigger issue may be that many writers just don’t know how to keep a better running log of their work to maintain all the relevant marginalia they’re actually producing. (Of course there’s also the subsequent broader librarian’s “[digital dilemma](http://boffosocko.com/2012/01/24/academy-of-motion-picture-arts-sciences-study-on-the-digital-dilemma/ "digital dilemma")” of maintaining formats for the future. As an example, thing about how easy or hard it might be for you to read that ubiquitous 3.5 inch floppy disk you used in 1995.)

A a technologist who has spent many years in the entertainment industry, I feel compelled to point everyone towards the concept of [**revision control**](http://en.wikipedia.org/wiki/Revision_control "revision control") (or version control) within the realm of computer science.  Though it’s primarily used in tracking changes in computer programs and is often a tool used by large teams of programmers, it can very easily be used for tracking changes in almost any type of writing from novels, short stories, screenplays, legal contracts, or any type of textual documentation of nearly any sort.

## Example Use Cases for Revision Control

### Publishing

As a direct example, I’m using what is known as a Git repository to track every change I make in a textbook I’m currently writing.  I can literally go back and view every change I’ve made since beginning the project, so though I’m directly revising one (or more) text files, all of my “marginalia” and revisions are saved and available.  Currently I’m only doing it for my own reference and for additional backup not supposing that anyone other than myself or an editor possibly may want to ever peruse it.  If I was working in conjunction with otheres, there are ways for me to track the changes, edits, or notes that others (perhaps an editor or collaborator) might make.

In addition to the general back-up of the project (in case of catastrophic computer failure), I also have the ability to go back and find that paragraph (or multiple pages) I deleted last week in haste, but realize that I desperately want them back now instead of having to recreate them de n0vo.

Because it’s all digital, future scholars also won’t have problems parsing my handwriting issues as has occasionally come up in differentiating Mary Shelley’s writing from that of her husband in digital projects like the [Shelley Godwin Archive](http://shelleygodwinarchive.org/ "Shelley Godwin Archive"). The fact that all changes are tracked and placed in a tree-like structure will indicate who wrote what and when and will indicate which changes were ultimately accepted and merged into the final version.

### Screenplays in Hollywood

One particular use case I can easily see for such technology is tracking changes in screenplays over time.  I’m honestly shocked that every production company or even more likely studios don’t use such technology to follow changes in drafts over time. In the end, doing such tracking will certainly make Writers Guild of America (WGA) arbitrations much easier as literally every contribution to a script can be tracked to give screenwriters appropriate credit. The end results with the easy ability to time-machine one’s way back into older drafts is truly lovely, and the outputs give so much more information about changes in the script compared to the traditional and all-too-simple (\*) which screenwriters use to indicate that something/anything changed on a specific line or the different colored pages which are used on scripts during production.

I can also picture future screenwriters using services like GitHub as platforms for storing and distributing their screenplays to potential agents, managers, and producers.

### Redlining Legal Documents

Having seen thousands of legal agreements go back and forth over the years, revision control is a natural tool for tracking the redlining and changes of legal documents as they change over time before they are finally (or even never) executed. I have to imagine that being able to abstract out the appropriate metadata in the long run may actually help attorneys, agents, etc. to become better negotiators, but something like this is a project for another day.

### Academia

In addition to direct research for projects being undertaken by academics like Neefs, academics should look into using revision control in their own daily work and writings.  While writing a book, paper, journal article, essay, monograph, etc. (or graduate students writing theses) one could use their own Git repository to not only save but to back up all of their own work not only for themselves primarily, but also future scholars who come later who would not otherwise have access to the “marginalia” one creates while manufacturing their written thoughts in digital form.

I can easily picture Git as a very simple “next step” in furthering the concept of the digital humanities as well as in helping to bridge the gap between [C.P. Snow’s “two cultures.”](http://boffosocko.com/2013/11/28/two-cultures/ "The Two Cultures") (I’d also suggest that revision control is a relatively simple step one could take before learning a particular programming language, which I think should be a mandatory tool in everyone’s daily toolbox regardless of their field(s) of interest.)

![Git Logo](https://i0.wp.com/boffosocko.com/wp-content/uploads/2014/04/Git-Logo-1788C.png?fit=910%2C380&ssl=1)

## Start Using Revision Control

“But how do I get started?” you ask.

Know going in that it may take parts of a day to get things set up and running, but once you’ve started with the basics, things are actually pretty easy and you can continue to learn the more advanced subtleties as you progress.  Once things are working smoothly, the additional overhead you’ll be expending won’t be too much more than the old method of hitting Alt-S to save one of your old Word documents in the time before auto-save became ubiquitous.

First one should start by choosing one of the myriad revision control systems that exist.  For the sake of brevity in this short introductory post, I’ll simply suggest that users take a very close look at [Git](http://git-scm.com/ "Git") because of its ubiquity and popularity in the computer science world and the fact that it includes a tremendously large amount of free information and support from a variety of sites on the internet. Git also has the benefit of having versions for all major operating systems (Windows, MacOS, and Linux). Git also has the benefit of a relatively long and robust life within the computer science community meaning that it’s very stable and has many more resources for the uninitiated to draw upon.

Once one has Git installed on their computer and has begun using it, I’d then recommending linking one’s local copy of the repository to a cloud storage solution like either [GitHub](https://github.com/ "GitHub") or [BitBucket](https://bitbucket.org/ "BitBucket").  While GitHub is certainly one of the most popular Git-related services out there (because it acts, in part, as the hub for a large portion of the open internet and thus promotes sharing), I often recommend using BitBucket as it allows free unlimited private but still share-able repositories while GitHub requires a small subscription fee for keeping one’s work private. Having a repository in the cloud will help tremendously in that your work will be available and downloadable from almost anywhere and because it also serves as a de-facto back-up solution for your work.

I’ve recently been playing around with version control to help streamline the writing/editing process for a book I’ve been writing. Though Git and it’s variants probably seem more daunting than they should to the everyday user, they really represent a very powerful tool. I’ve spent less than two days learning the basics of both Git and hosted repositories (GitHub and Bitbucket), and it has been more than well worth the minor effort.

There is a huge wealth of information on [revision control](http://git-scm.com/video/what-is-version-control "Video: What is Version Control?") in general and on installing and using Git available on the internet, including [full textbooks](http://git-scm.com/book "Pro Git by Scott Chacon"). For the complete beginners, I’d recommend starting with The Chronicle’s “[A Gentle Introduction to Version Control](http://chronicle.com/blogs/profhacker/a-gentle-introduction-to-version-control/23064 "A Gentle Introduction to Version Control | The Chronicle of Higher Education").” Keep in mind that though some of these resources look highly technical, it’s because many are trying to enumerate every function one could potentially desire, when even just the basic core functionality is more than enough to begin with. (I could analogize it to learning to drive a car versus actually reading the full manual so that you know how to take the engine apart and put it back together from scratch. To start with revision control, you only need to learn to “drive.”) Professors might also avail themselves of the use of their local institutional libraries which may host small sessions on learning such tools, or they might avail themselves of the help of their colleagues or students in the computer science department. For others, I’d recommend taking a look at Git’s primary website. BitBucket has an excellent [step-by-step tutorial](http://web.archive.org/web/20150810205530/https://confluence.atlassian.com/display/BITBUCKET/bitbucket+101 "BitBucket 101") (and troubleshooting) for setting up the requisite software and using it.

## What do you use for revision control?

I’ll welcome any thoughts, experiences, or additional resources one might want to share with others in the comments.