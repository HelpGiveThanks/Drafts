*How to make a whole Bug Genie like website one seamless collaboration tool with a common look and feel for all parts of the website: A) Home/Brochure Web Pages; B) Project Manger (The Bug Genie Solution/Tool/Sofware); C) Forum; and D) Wiki.  Click on link below to see before and after image of non-uniform vs uniform theme for all aspects of a website centered around The Bug Genie.*
[TBG Redesign.gif](http://forum.thebuggenie.com/download/file.php?id=230)

NOTE: These changes have been tested in 3.2.5.2 and should work in 3.2.6.  If you have made some or all of these changes to your 3.2.5.2 install and do not want to make them again to fix the security issues that 3.2.6 fixes, then see this post "What files need replacing from 3.2.6 to fix 3.2.5.2 security" http://forum.thebuggenie.com/viewtopic.php?f=1&t=1751 

**Post Overview**  
1. **Introduction**  
2. **[Project Manager = Frontpage](#Project-Manager-=-Frontpage)**   
3. **Issue Page**  
4. **Wiki**  
5. **Home/Brochure Pages**  
6. **Forum**  
7. **Code Changes**

##Introduction
The Bug Genie (TBG) 3.2.5 is the most well designed issue tracker I have found, and has enough project management tools to do the job I need done.  The fact that it is opensource (very, very much appreciated!), allowed me to redesign it to my liking.  I hope others will find my redesign ideas useful, and will improve upon them.  

*NOTE: thebuggenie.com website scope is for showing off The Bug Genie as a stand alone tool, not as a tool embedded in a larger website that to the average user appears to be part of an integrated website.  In my ignorance, I viewed the scope of the entire thebuggenie.com (A in the above image), issues/thebuggenie.com (B), and forum/thebuggenie.com (C) as one website. I wanted it, and was frustrated that by design it was not built to be integrated!  That is my frustration.  I am sure The Bug Genie team gave birth to The Bug Genie code out of frustration with existing bug trackers eleven years ago.  Point being, frustration is a good thing, and I am so very happy to join with other frustrated people in this open source movement to positively do something that results in a diversity of solutions (not one right way!).  In addition to my very small code contribution below, I donated money to thebuggenie.com project, and would encourage anyone reading this post to do the same, or buy a support ticket to help you (not do it for you) put the design changes I made below into your version of The Bug Genie: http://thebuggenie.com/support OR, Hey!, if you have loads of cash and are looking for a way to give back, hire The Bug Genie Team to make the design changes I made below an option offered with each new release of The Bug Genie!  I would if I could!* 

Before I get to my redesign, which includes making the whole Bug Genie website one seamless collaboration tool, I must let my respect be known, my sense of “WOW!” for the current design, and enthusiasm for the real and positive difference this tool must be making in the businesses and organizations using it.   The Bug Genie is a very intelligently designed tool with a Team (from what I have seen) focused on making the most content focused, uncluttered, Tufte-esk *(see quotes after the notes below)* quality-improvement-collaboration solution of its kind.  I picked TBG over other tools like Bugzilla, Mantis, and Trac because of how much care has obviously gone into helping the user understand what is on each screen.  I believe, my contribution below is only advancing a little of what The Bug Genie Team has already been working to accomplish, as evidenced by their own recent and incredible redesign effort documented and wonderfully illustrated in the following three blog posts: 
thebuggenie.wordpress.com/2012/03/15/so-what-does-it-look-like-part-1/
thebuggenie.wordpress.com/2012/04/02/so-what-does-it-look-like-part-2/
thebuggenie.wordpress.com/2012/04/04/so-what-does-it-look-like-part-3/  

*NOTE: All red letters and numbers added to screenshots relate to the lettered and numbered items below.  These lettered and numbered comments below may not make sense if you do not look at the screenshot pictures before reading them and while reading them. [Idea for labels came to me from here: Reinhold, Sealth (n.d.). Tufte’s Rules: 5 Use Labels [webpage]. Tufte’s Rules.  Copyright 2013 by the website. All rights reserved. Retrieved 6/12/2013 from http://www.sealthreinhold.com/tuftes-rules/rule_five.php] 

NOTE: All pictures below are hosted for free courtesy of imageshack.us, and sized to width 738px to maximize fit on this forum with one exception: the attached image below is too big to display legibly.  You must, and please do, click the link below to view it.  I posted a feature request to this forum to add an image re-sizer (with full size popup option): Image re-size MOD for forum to auto fit big images http://forum.thebuggenie.com/viewtopic.php?f=9&t=1690

FINAL NOTE (before I begin :-)): Please comment if you have ideas that would make this post better :idea: .*

My redesign was made following Edward Tufte's (EdwardTufte.com) rules for graphic design as I understand them.  They are not for everyone and every website!  Here are a couple of choice quotes by Tufte on website and software interface design: [quote]If possible, design architectures should be spare, straightforward, conventional, and self- effacing; AND the evidence presented should be rich, complex, multivariate, causal. The idea is to maximize the viewer's content reasoning time, and to minimize the design figuring out time and to reduce impediments to content reasoning. 

[Edward Tufte, Analytical design and human factors. retrieved 2/22/13 from http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0000KI [/quote]
[quote]Nearly all users come to a website for a content experience, not a designer experience.

[Edward Tufte, Good web design, web standards, user testing.  retrieved 2/22/13 from http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0000P9][/quote]  
Following from Tufte's design principles, two general design/usage problems with The Bug Genie tool and website focused my redesign efforts.  

First, The Bug Genie tool design while very appealing, draws my eye to unnecessary icons and columns of information, and to beautiful but unnecessary graphic elements that make it harder than necessary for me to focus on any page’s content.  Please click the image link below to see the overall changes I made to The Bug Genie design.  Top view is composed of four screenshots taken from the four areas of thebuggenie.com website that I redesigned, and the bottom view is screenshots of the same four areas on my website after the redesign.
[attachment=1]TBG Redesign.gif[/attachment]
Second, four essential elements at thebuggenie.com required to make the website work do not look like they are part of the same website and lack a standardized navigation interface (which frustrated me during my first few visits to the site when I was trying to learn about The Bug Genie).  These four essential elements are A) webpages describing what The Bug Genie is and what users can do on thebuggenie.com (essentially a brochure and a map of the entire website),  B) The Bug Genie tool itself (the star of the website), C) a forum to build community among Bug Genie users, and D) a wiki to provide documentation.  I’m not sure what to call a Brochure-Project Manger-Forum-Wiki website application, but a label is needed like CMS (content management system) to encourage the packaging of such a necessary suite of tools together.  Note that the redesign (click picture link above) allows for more content to be displayed in the same amount of space in addition to a uniform look and feel for all four elements.  It is more boring than the original, but perhaps some additional functionality could be added to the text box areas to spice things up with the ability to add youtube videos, image sliders, etc.?

The rest of this topic will be about each of the four elements before and after my redesigned to make them uniform, improve website navigation,  and focus users on content.  All the code changes I made to accomplish this redesign are posted last.  I’m a hack, and learned a lot while doing this, and in some cases redid my coding after learning of better ways, but my time is limited and with 192 hours invested in this redesign, I simply had to stop once it was working well and looked good, so please, improve my coding if you have the time (and critique my design changes too)!  

##Project Manager = Frontpage
Because The Bug Genie is the star of thebuggenie.com website, I am starting my redesign story with its Frontpage, followed by the Wiki, the Home page, and then the Forum. 
 
[img]http://imageshack.us/a/img832/3829/62626328.gif[/img]
[img]http://imageshack.us/a/img688/1893/92442432.gif[/img]
1) The Bug Genie logo is awesome and the name is really big.  Both are unnecessary to let users know what site they are on once they get past the home page.  So I removed the logo and name in my redesign to free up valuable top-menu space for essential navigation buttons.
2) The icons, like the home icon, duplicate the function of the text buttons.  They along with the logo distract my eyes from any page’s content.  I eliminated them to reduce distractions and to free up space.  
3) The ‘Frontpage’ button has a confusing name as the actual frontpage of the website is thebuggenie.com home page.  I changed the name of this button to ‘Project Manager’, which describes what this part of the website does. The Bug Genie’s powerful management tools make it much more than a bug tracker!  Mmm… perhaps that should be its tag line: The Bug Genie *much more than a bug tracker!*  In the code below, you’ll see I actually removed the frontpage button code, and created a new button that is [u]always[/u] available from the top menu, unlike the ‘Frontpage’ button which frustratingly disappears from the top-menu on some page views.  Perhaps this was due to a lack of space on the top-menu bar as some pages do require more buttons than other pages.  Plenty of space is created for all page buttons by removing the logo, website name, and unnecessary navigation menu-bar icons.  It is a boring solution, but as a user, I really like having primary-navigation buttons always available, especially when I am first learning to use and fall-in-love with a program.  
4) There are two types of dashboard buttons: a) user and b) project.  I kept accidentally pressing the user dashboard button when I really wanted the first-listed project’s dashboard.  So, I edited the code to rename the user dashboard button making it easier to tell it apart from project dashboard buttons.
4c) I could have used ‘Your Dashboard’ as the new label, but decided on the shorter ‘My Dashboard’ to save menu-bar space, and mainly because I like the more casual and friendly way ‘My Dashboard’ feels versus the more formal and cold ‘Your Dashboard.’   Anyway, I then had to change the phrasing everywhere else ‘Your’ is used to announce something is mine, as in the drop down menu under the user’s name.  See code changes below for all the places I made this change and let me know if I missed any, or got any wrong.
5) The yellow gradient is beautiful.  In fact, it is so eye-catching that it is the first thing that draws my attention on every page.  This gradient provides no information, and so I eliminated it.  (I have kept the blue gradient which is less eye catching, less distracting, and very nice looking.)
6) The ‘Quick links’ column provides essential navigation. I moved this navigation to the top-menu bar, freeing up valuable webpage space for content.
7) The ‘Home’ button is very important.  I moved this button to the top-menu bar and renamed it ‘Overview’, as this part of the website provides the user with an overview/brochure/map of both projects and website.
8) A permanent ‘Forum’ button is essential, so I moved it too to the top menu bar.
9) The blog link currently takes you to a dead end page that reads, *"Sorry, can't find that!  We couldn't find the page you wanted, are you sure you typed it right?"*  The function of the blog — announcements, news, etc. — can be done using the Forum or the Wiki, thus reducing information silos and improving website searchability.  Perhaps some of the graphical possibilities provided by the blog software can be added to the Bug Genie Wiki?
10) *(OK, please forgive the density of this next comment, but I really, really think such density is needed to illustrate why Serif fonts (http://en.wikipedia.org/wiki/Serif) are so important.)* Sans-serif fonts — Arial, Helvitica, etc. — have less information (no serifs!) than serif fonts — Times, Georgia, etc. — making large blocks of sans-serif text harder to read.  With serifs shaved off, like the shaved heads of army recruits, the brain has less information with which to identify words.  Basically, sans-serif fonts make words look uniform.  Large blocks of sans serif text, like large formations of soldiers, look nice when viewing entire text-blocks as a whole.  But, uniformity becomes a pain when you want to see the differences among words; when you want to read the words.  

(I believe san-serif fonts where initially used on the web because of low screen resolution.  Serif font letters get thin and wide in different places, unlike san-serif font letters, which are composed of uniform-width lines.  On low-res displays, the thin parts of serif letters actually disappear making serif letters harder to read than fully-visible, san-serif letters.  High resolution screens, such as the ones my user base owns, make serif letters fully visible.)

Due to the unique or messy appearance of serf text blocks, line spacing can be very dense, as it is easier to track what line you’re on when each line looks different, versus sans-serif lines of text, which look the same causing readers to lose their place in densely packed blocks of sans-serif text.  

Serif text blocks = more easily-readable content in less space (on high resolution screens).  

Serif fonts are very useful for titles, headers, and small blocks of text.  Combining san-serif titles and serif body text, helps me to better scan through headers on a page to find information blocks, and I think this combination looks really good.  Perhaps a toggle could be added to the configuration section to allow users to select serif or sans-serif fonts for body text, titles, etc?   
11) In the redesign, project descriptions appear below project names, instead of links to project websites and documentation.  At the thebuggenie.com below its main project name is a website link pointing to its home page, which is redundant navigation (thebuggenie.com ‘Home’ page button is also provided in its ‘Quick links’ column).  The documentation link wrongly informs users, “No documentation URL provided,” when documentation for the Bug Genie Project can be found by clicking the top-menu bar ‘Wiki’ button.  Perhaps in future versions these links and the project description could be toggled off and on project by project?

##**Issue Page**
12) The screenshots below contrast the top-menu bar and title area of the issue page before and after the redesign.  The primary three website buttons remain in view on the redesign (bottom), while on the default Bug Genie 3.2.5 issue page the #3 ‘Frontpage’, #8 ‘Forum’ and #7 ‘Home’ buttons are not available.  I removed the unnecessary #2 icon indicating issue type (next to the star) along with the other unnecessary icons, which made necessary space for the first three buttons on the top-menu bar. With these unnecessary icons and the #5 gradient removed, my eye focuses easily on the issue.  *NOTE: Even though there are more buttons on the top-menu bar in the redesign, the last button in the re-design 'Project Wiki' is further back then the same button in the current release of The Bug Genie.  More buttons! Less space!*
[img]http://img546.imageshack.us/img546/2135/51623631.gif[/img]

##**Wiki**
This is a wonderful feature allowing for searches that include both documentation and issues!  Forum integration would put all information related to projects in one searchable place, but would no doubt be a huge programming effort, and I am very grateful to have the Bug Genie as it is right now!  On to minor design changes to the wiki …
[img]http://imageshack.us/a/img825/9086/84007975.gif[/img]
[img]http://imageshack.us/a/img825/3145/49656269.gif[/img]
[img]http://imageshack.us/a/img831/4151/90716000.gif[/img]
13) I removed the links column to allow more space for content while in show mode.  I did not remove this column from edit mode, but I did reduce its width to allow for more space for content creation.  Perhaps this links column could be toggled on and off for each wiki page created, like the table of contents?
14) I changed the color of the ‘Table of contents’ box to light grey (showing up white due to the low resolution of the image).  The blue was much to good looking for its own good, drawing my eye away from the primary content.  I also changed the name of the box to ‘Page Overview’ as I think of a table of contents as referring to items on other pages of a book or magazine; not items on the table of contents page itself.  Also, I already used the word ‘Overview’ as a primary button for the website ‘Overview’ (aka’ Home’) page, so it made sense to refer to this box giving an overview of the page the name ‘Page Overview’.
15 and 16) For my needs, and to keep my community wiki-page creation uniform, I changed the code so that there are only two choices for header styles: ‘h1’ and ‘h2’.  I only point this out because you can see them in the screen shot, so I figured I needed to explain why there are only two header buttons.  You can see how I hacked the code below to achieve this.  I know there must be a better way! 

##**Home/Brochure Pages**
This was the hardest part of the design rethink on my part, because I felt a website requires a really amazing looking Home page (à la thebuggenie.com) and other brochure-like pages.  I tried to emulate the basic design of the buggenie.com by setting up my own website home page and brochure like webpages using Wordpress, Joomla, Doku Wiki (my favorite), and others.  It took me a while and several frustrating conversations with friends to figure out that the purpose of these webpages, no matter what tool renders them, is to provide users (especially first-time visitors and new users) a map of the site, brochure/executive summary of the site’s offerings, rules of participation (converse on the forum, report problems in the Bug Genie), etc.  Reluctantly, after setting up several mock home pages and not being satisfied with how they integrated with The Bug Genie, I decided to modify some Bug Genie Wiki pages to perform this function.  I ended up being very satisfied with the outcome.  The pages look good, look like part of my website, easily steer users to my Bug Genie, other collaboration tools, and to my software download links.  My 'Home' / 'Overview' wiki pages are not as exciting to view as say thebuggenie.com ‘Home’ and other brochure webpages, but I know that they will look better in the future as functionality is added to new versions of the The Bug Genie Wiki.  In addition, all the information on these pages is searchable by the Bug Genie, and permission access is controlled by the Bug Genie (no need for another web-tool for community members to log into to help improve the welcome-matt portion of the website).

*NOTE: I am using numbers I used above 3 ‘Project Manager’ or ‘Frontpage’,   4b release center via the project dashboard,   7 ‘Overview’ or ‘Home’,   8 ‘Forum’,   9 ‘Blog’ on the screenshots below, to show what buttons on thebuggenie.com home page need to be clicked to get to these essential parts of the website.*
[img]http://imageshack.us/a/img845/733/48978938.gif[/img]
[img]http://imageshack.us/a/img28/1453/74989867.gif[/img]
[img]http://imageshack.us/a/img832/7954/65261186.gif[/img]
3) On thebuggenie.com home page, the link to The Bug Genie is accessed by first clicking the ‘Help’ button and then scrolling down the help page to find The Bug Genie link which is labeled ‘online issue tracker’.  Because The Bug Genie is a core website tool, I moved it to the top-menu bar and re-labeled it ‘Project Manager’.  
4b) The ‘Get It’ button in the redesign is the release center of The Bug Genie on my website, which is accessed thru the project dashboard.  Individual links by project to the downloads-release center is on my overview/home page as part of the summary section for each project.  
7) ‘Home’ is retitled ‘Overview’ in the redesign.  The word 'Home' seemed to provide no real useful information other than telling users this page is the landing page for my website.  The word 'Overview' tells user's what they can expect to find on my landing page: an overview of the website and my projects.  I modified a Wiki page removing all tabs and most recent author information to make it feel more like a traditional landing page.  The link to this page is always available in the top-menu bar for lost and confused users.
8) The ‘Community’ and ‘News’ functions is performed in my redesign by the forum with news/blog as a forum section.  I think users should come to expect informal user-to-user or free user-to-developer help thru the forum and documentation type help from the wiki.  The buttons to the forum and wiki need to be in one consist place on the top-menu bar on every screen.   
9) As of the date of this post, the blog at thebuggenie.com has not received a new post since June 26, 2012, which makes me wonder if the project is being actively worked on, from just viewing the blog.  I know how much work it is maintaining news feeds, and wanted to make it easier on myself by eliminating the blog on my website.  There is really great information on the blog at the thebuggenie.com, but I see no reason why it could not be moved to the forum, thus helping the user better remember where they saw news announcements, and giving the impression of active upkeep by the developers.  
17) ‘Features’ goes to a beautifully designed brochure page at thebuggenie.com.  This page could be a wiki page.  I hope the ability to create columns in wiki pages is someday added to the text-creation tool for the Wiki.  Doku Wiki allows for html code to be used in its text areas.  Perhaps permissions to add html code by user type could be added to future versions of The Bug Genie, to insure security and allow for more imaginative wiki page creation by trusted users? 
18) Guest users in my redesign see a traditional home page, in that a more home page looking title with logo graphic is shown and the last author info and edit, history, etc. tabs are hidden.  Logged in users see a normal, editable, commentable wiki page.  I thought it important that new comers to the site feel like they are looking at a traditional home page, while logged in users feel invited to help improve the site by seeing that the site is about the business of continual quality improvement to both the projects and the website.  

##**Forum**
19) The only real design change is to the top-menu bar making the forum look and feel like a part the overall website.  
[img]http://imageshack.us/a/img600/4894/10sh.gif[/img]
[img]http://imageshack.us/a/img849/6848/11s.gif[/img]
I would recommend the Vanilla.com opensource forum over the phpBB forum tool used at thebuggenie.com, which I did try to make work for my website, along with Phorum (my second favorite, next to Vanilla), and SimpleMachinesForum (SMF) before finally deciding on Vanilla.  

Vanilla is a table-less forum with minimal icons and a layout design that gives most of the screen real-estate to the posts.  The plugins are also fantastic allowing users to login using gmail, twitter, etc. accounts among other wonderful things.    

If you view a Vanilla forum on a smart phone, the theme automatically changes to fit the smartphone’s screen!  In addition, the default color scheme of the Embed Theme which comes with the software looks great with the Bug Genie’s default color scheme.  I have included the code changes below to add the top-menu bar of the Bug Genie to the Vanilla forum’s Embed Theme.   NOTE: This is a hack in need of improvement!  But, it does work.  A better solution would be to create a custom theme meant to work with The Bug Genie and post it on the theme portion of the Vanilla website!  When I have time, I’ll do this unless someone beats me to it.  Anyone?  Anyone?  

Here are a couple of reviews/descriptions of Vanilla 2.0:
The forum is dead, long live Vanilla  http://boagworld.com/reviews/vanilla/ 
Vanilla Forums Review  http://www.forum-software.org/vanilla/review

I hope this post is taken as a sign of my great respect and appreciation for The Bug Genie and the website created to promote it and provide a platform for community participation.  I am committed to it (in that I needed all these elements for my website) and hope some of what I found useful for myself can be used to further improve what is already a very useful, and beautifully designed software tool.  

Cheers!  

David Matson

My code hacks are below.

##**Code Changes**
I learned a lot customizing The Bug Genie for my website.  Here is what I did to customize Bug Genie version 3.2.5.  If you want lots of help using this code for your site, I would recommend buying a support ticket from The Bug Genie Team.   

*NOTE: I used all caps sentences in the code to comment on what I discovered a section of code did or to comment on what my changes do.  Most of the time this all-caps text will be the only explanation provided for what I did.*

**Top Menu Bar**
*public_html/YOURBugGenieFolder/core/templates/headertop.inc.php*: do the following in this flie:

Replace the logo code which is the first few lines of code with the following code to create the Forum, Overview and Project Management buttons:

[code]
<?php // ADD THREE BUTTONS TO FRONT OF TOP MENU FOR FORUM, OVERVIEW WIKI PAGE, AND BUG GENIE FRONTPAGE ?>
		<div><nav class="tab_menu header_menu" id="main_menu">		
			<li>
		<div><a class= "tab_menu header_menu" id="main_menu" href="http://YOURSITE.COM/YOURBugGenieFolder/forumEmbed.html"> Forum</a>
		</li>
				<nav class="tab_menu header_menu" id="main_menu">		
			<ul>
			<li <?php if ($_SERVER["REQUEST_URI"] == '/YOURBugGenieFolder/thebuggenie/wiki/Overview'): ?> class="selected"><?php endif; ?>
			<?php if ($_SERVER["REQUEST_URI"] != '/YOURBugGenieFolder/thebuggenie/wiki/Overview'): ?> class="logo_name"><?php endif; ?>
			<div><a href="http://YOURSITE.COM/YOURBugGenieFolder/thebuggenie/wiki/Overview">Overview</a> </div></li>
		
		
		<nav class="tab_menu header_menu" id="main_menu">		
			<ul>
			<li <?php if ($_SERVER["REQUEST_URI"] == '/YOURBugGenieFolder/thebuggenie/'): ?> class="selected"><?php endif; ?>
			<?php if ($tbg_response->getPage() != 'home'): ?> class="logo_name"><?php endif; ?>
			<div><a href="http://YOURSITE.COM/YOURBugGenieFolder/thebuggenie">Project Manager</a> </div></li>
</div>[/code]
Delete png tags from the word image_tag to the period = image_tag($issuetype->getIcon() . '_tiny.png' ) .

Delete this line of code for all pulldown menus.  This action gets rid of triangle to right of menu items with pulldowns:
[code]
		<?php echo javascript_link_tag(image_tag('tabmenu_dropdown.png', array('class' => 'menu_dropdown'))); ?>
[/code]
Delete this line of code to remove the Frontpage menu item:
[code]
		<li<?php if ($tbg_response->getPage() == 'home'): ?> class="selected"<?php endif; ?>>
		<div><?php echo link_tag(make_url('home'), __('Frontpage')); ?></div></li>
[/code]
Change dashboard button:
[code]<?php // CHANGE STRING DASHBOARD TO MY DASHBOARD SO USER CAN SEE DIFFERENCE BETWEEN THEIR DASHBOARD BUTTON AND PROJECT DASHBOARD BUTTON ON BUG GENIE FRONTPAGE ?>
				<?php if (!$tbg_user->isThisGuest() && !TBGSettings::isSingleProjectTracker() && !TBGContext::isProjectContext()): ?>
					<li<?php if ($tbg_response->getPage() == 'dashboard'): ?> class="selected"<?php endif; ?>><div><?php echo link_tag(make_url('dashboard'),  __('My Dashboard')); ?> </div></li>
				<?php endif; ?>[/code]
*public_html/YOURBugGenieFolder/i18n/en_US/strings.inc.php* Add string My Dashboard and call it for User Dashboard button on main page (/ core / templates / headertop.inc.php) so user can see a difference between project and user dashboard buttons:
[code] $strings['My Dashboard'] = 'My Dashboard';[/code]
*public_html/YOURBugGenieFolder/modules/publish/templates/_menustriplinks.inc.php* remove this code from the file to get rid of wiki icon on menu header: 
[code]
image_tag('tab_publish.png', array(), false, 'publish')  .
[/code]
and change the top line of code to this
[code]
<li<?php if (($_SERVER["REQUEST_URI"] != '/YOURBugGenieFolder/thebuggenie/wiki/Overview') && ($selected_tab == 'wiki')): ?> class="selected"<?php endif; ?>>
[/code]
Delete this line of code in the file.  This action gets rid of triangle to right of menu items with pulldowns:
[code]
			<?php echo javascript_link_tag(image_tag('tabmenu_dropdown.png', array('class' => 'menu_dropdown'))); ?>
[/code]
Do not highlight the Wiki button if user is on Overview page
[code]<?php // changed first line of code adding in the url if question to keep the Overview wiki page from higlighting the wiki button in the header menu. ?>
<li<?php if (($_SERVER["REQUEST_URI"] != '/YOURBugGenieFolder/thebuggenie/wiki/Overview') && ($selected_tab == 'wiki')): ?> class="selected"<?php endif; ?>>[/code]

**Bug Genie !FrontPage (Project Manager main page)**
*public_html/YOURBugGenieFolder/modules/main/templates/index.html.php* Remove side bar code below so the sidebar does not show up. This allows for more room for the page content.
[code]
		<td class="side_bar">
			<?php include_template('main/menulinks', array('links' => $links, 'target_type' => 'main_menu', 'target_id' => 0, 'title' => __('Quick links'))); ?>
			<?php TBGEvent::createNew('core', 'index_left')->trigger(); ?>
		</td>[/code]
*public_html/YOURBugGenieFolder/modules/project/templates/_overview.inc.php* delete this line of code to remove project icons:
[code]
 		<?php echo image_tag($project->getSmallIconName(), array('style' => 'float: left; margin: 3px 5px 0 0; width: 16px; height: 16px;'), $project->hasSmallIcon()); ?>
[/code]
Then delete this code to remove text about external project websites.
[code]
			<?php if ($project->hasHomepage()): ?>
			<a href="<?php echo $project->getHomepage(); ?>" target="_blank"><?php echo __('Go to project website'); ?></a>
		<?php else: ?>
			<span class="faded_out" style="font-weight: normal;"><?php echo __('No homepage provided'); ?></span>
		<?php endif; ?>
		|
		<?php if ($project->hasDocumentationURL()): ?>
			<a href="<?php echo $project->getDocumentationURL(); ?>" target="_blank"><?php echo __('Open documentation'); ?></a>
		<?php else: ?>
			<span class="faded_out" style="font-weight: normal;"><?php echo __('No documentation URL provided'); ?></span>
		<?php endif; ?>
[/code]
Add this code to show project descriptions:
[code]<?php   // ADD getDescription CODE TO ADD PROJECT DESCRIPTION TO EACH PROJECT ON MAIN PAGE TO SHOW PROJECT DESCRIPTION 
		?>
		<span class="faded_out" style="font-weight: normal;"> <?php echo ($project->getDescription()); ?> </span>[/code]
On the !FrontPage if Bug Genie is set to show summary status per issue types, then !FireFox displays the closed and reported project number totals aligned left instead of relative to the green bars.  
I found the following article at [http://stackoverflow.com/questions/5148041/does-firefox-support-position-relative-on-table-elements StackOverflow] explaining that Firefox requires a <div style> tag instead of the <td style> tag currently in line 51 of the modules/project/templates/_overview.inc.php file released with version 3.2.5 ([http://issues.thebuggenie.com/thebuggenie/issues/1924 filed this as issue 1924 with main Bug Genie project]).   
Current code for line 51 is
[code]<td style="padding-bottom: 2px; width: auto; position: relative;">[/code]
Fixed code for line 51 is
[code]<td><div style="padding-bottom: 2px; width: auto; position: relative;">[/code]
And then a </div> tag needs to be added to line 63
[code]</div></td>[/code]
Add the follow code to the div style tag for project_names as shown below: padding: 8px 0 0 0
[code]
	<div class="rounded_box <?php if (!($project->isIssuelistVisibleInFrontpageSummary() && count($project->getVisibleIssuetypes()))): ?>invisible <?php else: ?> white borderless <?php endif; ?>project_strip">
	<div style="float: left; font-weight: normal; 
	<?php   // ADD PADDING CODE TO REDUCE SPACING BETWEEN GREEN BARS AND PROJECT NAMES ON MAIN PAGE //   ?>   padding: 8px 0 0 0">
[/code]


**Footer**
*public_html/YOURBugGenieFolder/core/templates/footer.inc.php* 
[code]<?php // BEGIN ADD CONTENT AND LINKS TO FOOTER ?>
				<?php echo __('Project manager and wiki by %thebuggenie%', array('%thebuggenie%' => '<a href="http://YOURSITE.COM/YOURBugGenieFolder/thebuggenie/about"  target="_blank">The Bug Genie</a>')); ?>.
				<?php echo __('Forum by %link_to_MPL%', array('%link_to_MPL%' => '<a href="http://vanillaforums.org/"  target="_blank">Vanilla.org</a>')); ?>.
				
								<?php echo __('Content copyright (except where noted) =
 %link_to_MPL%', array('%link_to_MPL%' => '<a href="http://creativecommons.org/licenses/by/3.0/"  target="_blank">Creative Commons Attribution 3.0</a>')); ?>.
<?php // END ADD CONTENT AND LINKS TO FOOTER ?>  [/code]


**Wiki Pages**
*public_html/YOURBugGenieFolder/modules/publish/templates/_articledisplay.inc.php* Put in code so author and last update only shows if user is logged in.  This makes guest users see a more traditional looking website information page.
[code]<?php // DO NOT SHOW AUTHOR AND UPDATE INFO IF USER IS NOT LOGGED IN ?>
<?php if (!$tbg_user->isGuest()): ?>
<?php // CHANGE WORDING Last updated at TO Updated ?>			
			<?php echo __('Updated %time%, by %user%', array('%time%' => tbg_formatTime($article->getPostedDate(), 3), '%user%' => '<b>'.(($article->getAuthor() instanceof TBGIdentifiable) ? '<a href="javascript:void(0);" onclick="TBG.Main.Helpers.Backdrop.show(\'' . make_url('get_partial_for_backdrop', array('key' => 'usercard', 'user_id' => $article->getAuthor()->getID())) . '\');" class="faded_out">' . $article->getAuthor()->getName() . '</a>' : __('System')).'</b>')); ; ?>
<?php	
//removed category code lines 21 to 66 in version 3.2 4 for wiki pages so user does not see grey box before comments section telling them the article is not in any categories. Leave this in if you plan on using the category feature.  I am building such links into my wikipages and find the category feature to be just anohter navigation interface that migh confuse users.
?>[/code]

*public_html/YOURBugGenieFolder/modules/publish/templates/_header.inc.php* 
[code]<?php $article = (isset($article)) ? $article : null; ?>
<?php // CHANGE STYLE OF WIKI TITLE IF USER IS GUEST ?>
<?php if (!$tbg_user->isGuest()): ?> <div class="header tab_menu"   > 
<?php else: ?>
		<div class="guest"   >

<?php endif; ?>


<?php // BEGIN ONLY SHOW EDITING TABS IF USER IS LOGGED IN ?>
<?php if (!$tbg_user->isGuest()): ?>

...

link_tag(make_url('publish_article_permissions', array('article_name' => $article_name)), __('Permissions')); ?></li>
					<?php endif; ?>
					<li<?php if ($mode == 'attachments'): ?> class="selected"<?php endif; ?>><?php echo link_tag(make_url('publish_article_attachments', array('article_name' => $article_name)), __('Attachments')); ?></li>
				
			</ul><?php endif; ?><?php endif; ?>
		<?php endif; ?>
	<?php endif; ?>
<?php // END ONLY SHOW EDITING TABS IF USER IS LOGGED IN ?>

...

	<?php elseif (mb_substr($article_name, 0, 9) == 'Category:'): ?>
		<span class="faded_out blue">Category:</span><?php echo get_spaced_name(mb_substr($article_name, 9)); ?>
	<?php else: ?>	
	
<?php // IF USER IS LOGGED IN SHOW OVERVIEW WIKI TITLE AND IF GUEST SHOW TITLE BELOW ?>
		<?php if ($_SERVER["REQUEST_URI"] != '/YOURBugGenieFolder/thebuggenie/wiki/Overview'): ?><?php echo get_spaced_name($article_name); ?> <?php else: ?>
		<?php if ($tbg_user->isGuest()): ?>  
			<div class="guest_overview_page"><?php echo image_tag(TBGSettings::getHeaderIconUrl(), array('style' => 'max-height: 24px;'), TBGSettings::isUsingCustomHeaderIcon()); ?><br> 		
 <?php echo "Welcome to the Help Give Thanks Beta Project Website!"; ?> <br> <span  style="font-size: .7em" ><?php echo "Feel free to look around.  Website testing and content editing in progress."; ?></span></div>
		<?php else: ?>
		 <?php echo "Help Give Thanks Project Overview"; ?><?php endif; ?>
<?php endif; ?>
<?php
 // END IF USER IS LOGGED IN SHOW OVERVIEW WIKI TITLE AND IF GUEST SHOW TITLE BELOW 
?>[/code]

*public_html/YOURBugGenieFolder/modules/publish/templates/showarticle.html.php*  Remove side bar when showing wiki articles.
[code]<?php
// TURNED OFF SIDER BAR				
//				<td class="side_bar">
//			<?php include_component('leftmenu', array('article' => $article)); TOOK OUT QUESTION MARK SYMBOL > 
//		</td> ?>[/code]


**Issue Page**
public_html/YOURBugGenieFolder/modules/main/templates/viewissue.html.php
[code]					<?php /* DO NOT SHOW ISSUE TYPE IMAGE ?>
					<td class="title_left_images">
						<?php echo image_tag((($issue->hasIssueType()) ? $issue->getIssueType()->getIcon() : 'icon_unknown') . '_small.png', array('id' => 'issuetype_image')); ?>
					</td>  < */ ?>[/code]


**Text Editor Header Buttons**
*public_html/YOURBugGenieFolder/thebuggenie/iconsets/oxygen/markitup* in this folder comment out h2.png, h4.png, and h5.png files adding 'OLD' to file name.  Change image of h3 file to h2 files image = H2.  This will show user only the h1 and h2 buttons, which helps to define headers to two possibilities, which I find to be enough to keep things uniform.

*public_html/YOURBugGenieFolder/thebuggenie/js/thebuggenie.js* change what header buttons do in textbox editor by changing code to:
[code]TBG.Main.Helpers.MarkitUp = function(element) {
	element.markItUp({
		previewParserPath:	'', // path to your Wiki parser
		onShiftEnter:		{keepDefault:false, replaceWith:'\n\n'},
		markupSet: [
			{name:'Heading 1', key:'1', openWith:'====== ', closeWith:' ======', placeHolder:'Your title here...'},
			{name:'Heading 1', key:'2', openWith:'====== ', closeWith:' ======', placeHolder:'Your title here...'},
			{name:'Heading 2', key:'3', openWith:'======= ', closeWith:' =======', placeHolder:'Your title here...'},
			{name:'Heading 2', key:'4', openWith:'======= ', closeWith:' =======', placeHolder:'Your title here...'},
			{name:'Heading 2', key:'5', openWith:'======= ', closeWith:' =======', placeHolder:'Your title here...'},[/code]


**Main CSS File Changes = oxygen.css**
*public_html/YOURBugGenieFolder/thebuggenie/themes/oxygen/oxygen.css* Changes made to this file are indicated in attached file below.


**Wiki CSS File Changes = publish.css**
*public_html/YOURBugGenieFolder/thebuggenie/themes/oxygen/publish.css* made the following changes to the formatting specified in the file:

[code].toc .publish_toc_3 { margin: 0 0 3px 7px; font-weight: bold; font-size: 1.2em; font-family: 'Open Sans', sans-serif;} /*changed font family and size for wiki table of conents primary items*/ 

.toc .publish_toc_6 { margin: 0 0 3px 26px; font-size: 1.2em; font-family: 'Open Sans', sans-serif;} /*changed font family and size for wiki table of conents secondary items*/ 

.article h6 { font-size: 1.0em; padding: 3px 3px 3px 0; } /*changed font size for wiki secondary article titles*/ 

#article_comments h4 { color: #888; border-top: 1px solid #CCC ; padding: 5px 5px 5px 0; } /* Changed: added line (border) */

.article .header { margin: 2px 0 5px 0; color: #777; padding: 0px; font-weight: bold; font-size: 17px; border-bottom: 1px solid #CCC; } /*changed font color and padding indent*/[/code]


**Language Changes PHP**
*public_html/YOURBugGenieFolder/modules/publish/fixtures/DefaultWorkflow* change 'Not a bug' TO 'Not an issue'

*public_html/YOURBugGenieFolder/modules/publish/fixtures/WorkflowDefault* change 'Not a bug' TO 'Not an issue'

*public_html/YOURBugGenieFolder/core/classes/TBGStatus.class.php* 'Not a bug' TO 'Not an issue'

*public_html/YOURBugGenieFolder/modules/publish/templates/_toc.inc.php* Change spelling of 'Table' to 'Teble' in 2 strings so they match the strings in the English string file.  ([http://forum.thebuggenie.com/viewtopic.php?f=11&t=1652 logged this issue] in main Bug Genie project forum).
[code]<?php // CHANGE SPELLING OF TABLE TO TEBLE TO CALL UP CORRECT STRINGS ?>
	<div class="header"><a href="javascript:void(0);" onclick="$('publish_toc').toggle();"><?php echo __('Teble of contents'); ?></a></div>
	<div class="faded_out"><?php echo __('Move your mouse here to toggle the teble of contents'); ?></div>[/code]
*public_html/YOURBugGenieFolder/i18n/en_US/strings.inc.php* Make the following changes to strings (Change spelling of 'Table' to 'Teble' in 2 strings so they match the strings in the _toc.ini.php file above.  ([http://forum.thebuggenie.com/viewtopic.php?f=11&t=1652 logged this issue] in main Bug Genie project forum).:

[code]$strings['Move your mouse here to toggle the teble of contents'] = 'Move your mouse here to toggle page overview'; 

$strings['Teble of contents'] = 'Page Overview';

$strings['Frontpage'] = 'Project Manager';

$strings['Your account'] = 'My account';

$strings['Your projects'] = 'My projects';

$strings['Your saved searches for this project'] = 'My saved searches for this project';

$strings['Your dashboard'] = 'My dashboard';

$strings['Your drafts'] = 'My drafts';

$strings['Your issues'] = 'My issues';

Include this string if you want the following help to appear below your text boxes for reminding users how to create internal links to issues and wiki project pages:
  
$strings['To auto-link to an existing issue, write "issue", "bug", "ticket" or the issue type (like "bug report" or "enhancement") followed by the issue number (ex: "%ticket_example_1%" or "%ticket_example_2%"). Enclose sourcecode samples in <source></source> tags.'] = 'Link to an existing issue = issue + space + alpha-# OR issue HGTS-8. Link to wiki page (which will create a new page when clicked if it does not yet exist) = TwoOrMoreCapitalizedWordsStuckTogether OR [[double bracketed word]]. Link to project wiki page = [[ + Project Name + : + WikiPageName + ]] OR [[Project Name:Name]] USE double brackets ONLY for single word names, as you will get_words_with_lines_between_them! DoubleWord names with no space will get a space between words when wiki page is created (and_no_lines).';[/code]

Triage Question for Prioritizing Problem Issues
[code]
  $strings['Crash: Bug causes crash or data loss / asserts in the debug release'] = '7 Crash: Problem results in crash, data loss, freeze that requires quit and restart of solution, etc.';
  $strings['Major usability: Impairs usability in key scenarios'] = '6 Documentation: Problem in documentation or lack of documentation makes use impossible, too time consuming, too confusing, etc.';
  $strings['Minor usability: Impairs usability in secondary scenarios'] = '5 Major usability Problem: Problem impairs usefulness in a sequence of actions necessary to complete a primary process — a major reason for using the solution.';
  $strings['Balancing: Enables degenerate usage strategies that harm the experience'] = '4 Minor usability problem: Problem impairs usefulness in a sequence of actions necessary to complete a secondary process — a minor reason for using the solution.';
  $strings['Visual and Sound Polish: Aesthetic issues'] = '3 Too much freedom: Problem allows people using the solution to make preventable mistakes.  More structure is needed to set people up for success.';
  $strings['Localization'] = '2 Look and Feel: Problem of design, placement of things (text, titles, graphics, etc), not enough gray/color contrast, other esthetic issues, etc.';
  $strings['Documentation: A documentation issue'] = '1 Language Problem: Need more universally understood English words, better wording, or other language version — like Arabic, Hindi, Mandarin, Portuguese, Spanish, etc.';
  $strings['Blocking further progress on the daily build'] = '5 Problem requires priority-fast-fix.  Anyone using the solution will feel like giving up on it when this problem happens to them.';
  $strings['A User would return the product / cannot RTM / the team would hold the release for this bug'] = '4 Must fix in next version.  Invested users will continue to use the solution despite major pain.  Less committed will stop using the solution.';
  $strings['A User would likely not purchase the product / will show up in review / clearly a noticeable issue'] = '3 Problem is clearly noticeable and painful.  Least invested and new users may stop using solution, but not people mildly or fully invested.';
  $strings["A Pain – users won't like this once they notice it / a moderate number of users won't buy"] = '2 A Pain when noticed, but bearable for all but the least invested in the solution.';
  $strings['Nuisance – not a big deal but noticeable / extremely unlikely to affect sales'] = '1 Nuisance. Not a big deal, but noticeable. Extremely unlikely to be a reason for anyone to stop using the solution.';
  $strings['Will affect all users'] = '5 Affects nearly everyone.  Problem is very easy to come across.';
  $strings['Will affect most users'] = '4 Affects most. Problem is pretty easy to come across, and about 2/3 will suffer because of it.';
  $strings['Will affect average number of users'] = '3 Affects 50%.  Problem will happen to about half those using the solution.';
  $strings['Will only affect a few users'] = '2 Affects a few.  Problem is somewhat difficult to encounter, etc. and only a 1/3 will see it.';
  $strings['Will affect almost no one'] = '1 Affects almost no one.  Problem is very well hidden.  Only a teeny, tiny fraction will be unlucky enough to be troubled by it.';
[/code]

Triage Question Labels for Prioritizing Problem Issues
[code]
  $strings['Triaging: Bug type'] = 'Type of Problem';
  $strings['What type of bug is this?'] = 'What type of problem is this? For example is it a crashing issue, a problem with documentation, a matter of look and feel, etc.?';
  $strings['Triaging: Likelihood'] = 'Likelihood of Experiencing Problem?';
  $strings['How likely are users to experience the bug?'] = 'How likely is someone to encounter this problem? Will everyone run into it?';
  $strings['Triaging: Effect'] = 'How Painful is this problem?';
  $strings['Of the people who experience the bug, how badly does it affect their experience?'] = 'Of the people who experience the problem, how painful is this experience?';
[/code]

Spacing of Triage Questions for Priortizing Problem Issues
*public_html/YOURSITE.COM/YOURBugGenieFolder/modules/main/templates/_reportissue.inc.php* change label spacing for a better fit, look, etc. from 180px to 160px for first label, 320px for second, and 260px for third label.  You'll see change after update label text in the $string file below.
[code]

<td style="width: 160px;"><label for="pain_bug_type_id" id="pain_bug_type_label"><span>* </span><?php echo __('Triaging: Bug type'); ?></label></td>

<td style="width: 320;"><label for="pain_likelihood_id" id="pain_likelihood_label"><span>* </span><?php echo __('Triaging: Likelihood'); ?></label></td>

<td style="width: 260px;"><label for="pain_effect_id" id="pain_effect_label"><span>* </span><?php echo __('Triaging: Effect'); ?></label></td>

[/code]



**Language Changes MySQL**
UPDATE MYSLQL Database `your_buggenie` TABLE`tbg3_listtypes` SET `name` = 'Not a bug' TO 'Not an issue' WHERE `tbg3_listtypes`.`id` =26;

**##Vanilla Code Additions to Add Bug Genie Style Header and Main Navigation Buttons: Forum, Overview, Project Manager**

*public_html/YOURVanillaForumFolder/themes/EmbedFriendly/views/default.master.tpl* add the table below right after the first body tag as shown below.

[code]<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en-ca">
<head>
  {asset name='Head'}
</head>
<body id="{$BodyID}" class="{$BodyClass}">

<table style="font-size: 0.98em; font-family: 'Open Sans',sans-serif; width: 100%; height: 28px;" cellpadding=0 cellspacing=0>
	<td style="padding-top: 7px; background: #FAF3B8; width: 1%;" >				
		<a style="vertical-align: middle; padding: 5px; font-weight: bold; color: #000000; " href="http://YOURSITE.COM/YOURVanillaForumFolder/">Forum</a>
	</td>						
	<td> 
		<div  id="TopMenu_gradient" style="
		padding-top: 7px;
		height: 28px;
		background: #6193cf; /* Old browsers */ ; 
		background: -moz-linear-gradient(top, #6193cf 0%, #396ba7 100%); /* FF3.6+ */;
		background: -khtml-gradient(linear, left top, left bottom, from(#6193cf), to(#396ba7)); /* KHTML */;
		background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,#6193cf), color-stop(100%,#396ba7)); /* Chrome,Safari4+ */;
		background: -webkit-linear-gradient(top, #6193cf 0%,#396ba7 100%); /* Chrome10+,Safari5.1+ */;
		background: -o-linear-gradient(top, #6193cf 0%,#396ba7 100%); /* Opera11.10+ */;
		background: -ms-linear-gradient(top, #6193cf 0%,#396ba7 100%); /* IE10+ */;
		filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#6193cf', endColorstr='#396ba7',GradientType=0 ); /* IE6-9 */;
		background: linear-gradient(top, #6193cf 0%,#396ba7 100%); /* W3C */;
		"/> 
		<a style="margin-left: 20px; color: white;" href="http://YOURSITE.COM/YOURBugGenieFolder/thebuggenie/wiki/Overview">Overview </a>
		<a style="margin-left: 20px; color: white;" href="http://YOURSITE.COM/YOURBugGenieFolder/thebuggenie">Project Manager &nbsp;  &nbsp; </a>
		</div>
	</td>
</table>[/code]
