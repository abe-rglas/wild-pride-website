# website exit report

## the practical advice
Unfortunately the learning curve is a bit steep for self-hosted websites. Unlike in wordpress, there is no simple web interface to make edits to the site. Instead, I make changes from a text editor on my computer. Ideally, the person to maintain the website would know, or should learn:
* Basic CSS. I recommend the Mozilla tutorial for learning CSS, since it explains the underlying logic of CSS.
* HTML. You can also use the Mozilla tutorial!
* Any static site generators - others include 'Hugo', 'Jekyll', etc. They're all pretty similar to each other.
* Javascript. I learned on the job. The only javascript code I have is for the interaction triangle buttons.

## the moving parts
The domain name - wildpride.ca - is a subscription service with porkbun. They charge us around $ 30 every year.

The website itself is hosted with Koumbit. Koumbit has a web interface called AlternC to make changes to the website - for example, to connect the domain name to the site itself. Once the website was set up, I didn't really log into AlternC after that.

When I've made changes on my computer and I want them to be shown on the website, I ran the following commands:
"lftp -c 'open -u wpmtl_abe, [my password] ftp.koumbit.net; mirror -R _ site" , except I wrote my actual password instead of [my password]. 

As well as having the website on my computer, I've uploaded it to github, so that other people can copy the website or make changes to it.

## the directory structure of the website
I used the static site generator "eleventy". Documentation for it can be found here: https://www.11ty.dev/docs/.

On my computer, I have a folder for the website. It has a "content" folder that has files for each page, a "css" folder dedicated to the stylistic parts of the website (font, text color, etc), an "assets" folder for images, and an "_ includes" folder that has different templates. What eleventy does is applies the templates in "_ includes" to my content folder, and it generates html files - what ends up displayed on a browser - to the "_ site" folder. I never manually change the "_ site" folder; it's the output of my other folders. 

Within content, the "dates" folder has all the files for each event. Newer events just have one markdown file ("filename.md") whereas older ones have a markdown file and a json file with the metadata (since this was before I learned that I could just put metadata in the one markdown file).

## the credentials
For the domain names, wildpride.ca and fierteindomptable.ca:
URL: porkbun.com
Username: wildpride
Password: 4-!3tFE-X3@7

For the site management - putting it on line, etc.
URL: bureau.koumbit.net
Username: wpmtl
Password: LF9k":Wm'8pdV"P

## get in touch with me!
Email: aberglas@yorku.ca
Whatsapp: 613-322-3193. I don't have notifications, so it can take me a week or so to see the message. You can also text me regularly to ping me to check Whatsapp.

