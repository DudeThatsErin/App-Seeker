---
{"title":"1Password","dg-publish":true,"dg-updated":"2023-08-10T09:25","dg-created":"2023-08-04T09:00","dg-path":"Password Managers/1Password.md","dg-permalink":"pw-managers/1password","author":"Erin Skidds","authorURL":"https://github.com/DudeThatsErin","editor":null,"editorURL":null,"URL":"https://1password.com","aliases":["one password","pw","1pw"],"tags":["passwords","management"],"apps":["android","iOS","linux","macOS","web","windows","command line"],"openSource":null,"worksOffline":true,"multiDeviceSync":true,"storageAmount":1,"addlStorage":null,"totpStorage":true,"pwSharing":true,"2FAoptions":true,"noFamily":5,"addFamily":true,"noBusiness":10,"addBusiness":true,"hq":"Toronto,CA","serverLocation":"","priceURL":"https://1password.com/business-pricing","monthPrice":null,"yearPrice":35.88,"freeOption":false,"otpOption":false,"otpPrice":null,"anyDiscounts":true,"discountDescription":"40% off Individual Accounts & 50% off Families Account with CyberNews Coupons","discountURL":["https://start.1password.com/sign-up/individual?c=CYBER40&cjevent=e56cd90716cb11ee80ba005d0a82b824&utm_medium=affiliate&utm_source=Adtech+lt%2C+UAB&utm_campaign=5596782&utm_content=100242223&utm_term=Cyber+News%3A+Enjoy+40%25+Off+Individuals+at+1Password%21+New+Customers+Only%21&cjdata=MXxOfDB8WXww","https://start.1password.com/sign-up/?l=en&c=CYBER23&cjevent=19da89c616cc11ee812cef7b0a82b82d&utm_medium=affiliate&utm_source=Adtech+lt%2C+UAB&utm_campaign=5596782&utm_content=100242223&utm_term=Cyber+News%3A+Enjoy+50%25+Off+Families+at+1Password%21+New+Customers+Only%21&cjdata=MXxOfDB8WXww"],"permalink":"/pw-managers/1password/","dgPassFrontmatter":true,"created":"2023-08-04T09:00","updated":"2023-08-10T09:25"}
---

# Pros & Cons
## Pros
- Modern Interface with drag & drop capabilities.
- Ability to save social media logins for websites.
- Multiple avenues of support (reddit, twitter, their forum, and email)
- More templates for saving items.
- Shared vaults to easily share items between accounts. 
## Cons
- Expensive at $60/year for Families and $36/year for Individuals.
- Super Buggy (read below on the bugs I have experienced)
- Confusing to organize items between vaults, categories, and tags.
- Support via email is super slow. They only email once, maybe twice, a day.
- Sharing vaults can only be done via the web vault. You cannot do that via the apps.

# Our Review
[1Password](https://1password.com/) is one of the top password managers out there. It is made for business, personal, enterprise and developer use. It has features that [[Digital Gardens/Tools/Password Managers/Bitwarden\|Bitwarden]] does not have like saving GitHub Secrets, SSH Secrets/Keys, and more. In my review, I’m going to be going over why I decided to use Bitwarden over 1Password and what I think about it as a developer.

![1PasswordBlank.png](/img/user/Digital%20Gardens/Tools/images/1PasswordBlank.png)
1Password is a great application, don’t get me wrong. There are millions of people and “over 100,000 businesses” that use it (according to 1Password).
## Is 1Password glitchy/buggy?

Yes. Very much so. Especially if you are using the beta extension or application(s). Now, as a developer, I know beta = bugs. That is a given. I don’t mind them because I _hope_ they will get ironed out before they hit production.

So, after I had enough of the bugs in the betas I swapped and only used production. Production is _better_ but it still has A LOT of bugs. You can read about the bugs if you go into any of the sections of their [Support Community](https://1password.community/). These are all from people reporting issues publicly to 1Password.

I believe it is so glitchy/buggy because 1Password is cluttered with features and none of those features are without bugs. Some of the bugs I’ve faced are:

- Not being able to login to Discord mobile client without opening the 1Password app. Autofill doesn’t work. Though this may be a Discord issue cause BW is in and out on this page but still works better so that is why I am including it here.
- Usernames/Autofills not showing up above the keyboard when the URL matches what is in 1Password.
- Not popping up after logging in to save username/password. BW is known for not doing this so I don’t worry about it cause I add my logins to it _before_ logging in. 1Password is known for their pop up (similar to LastPass) but that does not come up all of the time and when it doesn’t, if you generated a password and didn’t save the password first, you are screwed.
## Any other annoyances?
Yes, it is confusing how to sort items because you have…

- Vaults -> These can be used to separate logins and different items you have saved from one another so you can have a “Work” vault for work passwords and a “Home” vault for all of your other ones. Then you can filter which one is shown in the browser extension or desktop app or vice versa. Plus, you can share vaults with other 1Password users if you have a family account and they can see and update those passwords as well.
- Categories -> These contain the different types of items you have saved in your vault. “Login”, “Notes” and “Cards” are just some of the few types.
- Tags -> Just like anywhere else, an item can have one ore more tags. Tags can be uppercase or lowercase and are generally 1 word.

and the list goes on…

So, I never knew how to sort my passwords. Plus, when you try to use tags, when you are initially saving items you aren’t suggested tags. So, in your left sidebar you can have “Shopping”, “shopping”, and “SHOPPING”, etc. depending on how you typed it at the time. Then you have to go through and edit all of the items under each tag to combine and delete the extra tags. It is super annoying.  
It has been brought up [on their official forums](https://1password.community/discussion/129002/tag-list-and-or-autocomplete-suggestions-in-save-new-item-popup) back in April of 2022 with an “internal feature request opened for it” over a YEAR ago. No updates. If they really cared about this feature, it would have been added by now.

This next issue I have to preface & it will be long because it is a fresh issue that I am having.

I have used 1Password’s Families account with my mom, my youngest sister, and my dad. Before I originally switched to the GitHub Student Individual account after it was released I assumed that the login date inside 1Password’s online account (where you can see your family members) was the last time they logged into the system. So, having not seeing anyone logged in, in over a month, I figured they were signed up but not using it. So, I switched. Something I regret.

They provided me a credit of $33.70 to my account for the unused time on my 1Password Families account and had me downgrade and I was able to sign up for the GitHub Student Individual account. Now, I can’t see the credit in my account but I’ve had like 4-5 people (at this point) confirm.

My mom contacted me around the end of May (about 3 weeks prior to this update, dated above) saying she was unable to login. So, I suggested to contact them but she just said to forget it and she went back to using pen & paper.  
Then about a week ago my father contacted me saying the same thing. He wanted me to pursue them. So I did.

No one informed me prior to downgrading that I wouldn’t be considered a new customer if I needed/wanted to upgrade again. My $33.70 credit is stuck in the 1Password account. They will not refund it.  
They are willing to upgrade me to Families but I would be out $36+ as families is $60/year and the families account date would restart. All I want them to do is to reset me back to how I was before I signed up for the GitHub Student Individual account with the same expiration date. They will not. It isn’t like they would lose any money in the process. GitHub was free… Resetting back to the original expiration date doesn’t lose them any money. They are just being greedy.  
It puts a bad taste in my mouth. Horrible taste.

I 100% realize this was _my_ fault for assuming they weren’t using it… I get that. I shouldn’t have changed anything in the first place. I take full responsibility. There have been other times with other companies that they have happily done this for me because it loses them ZERO dollars. Literally nothing changes. Just settings in a system.  
Yet, 1Password is unwilling to? It makes no sense.

Also, going through this process I have found that you can expect a reply to your ticket around 8-10am EST and then assuming you reply within minutes, you can get 1 more reply around 1-5pm EST. That is ALL each day. _Sometimes_ you may be able to squeeze 1 more but that is rare. Also, the 2nd reply is not guaranteed. Sometimes that becomes their first reply and you only get 1 reply that day. It is VERY slow. So if anything goes wrong with your account (billing or otherwise) you are screwed if Reddit goes under (may happen) or is unhelpful and no one is helping on their forums.
## Are there any good things about 1Password then?

Oh, most definitely. The app has a modern look versus the dated look [Bitwarden](https://dudethatserin.com/bitwarden-review/) still has (even after the refresh). 1Password can also save your SSH Keys so you can use them to login to your accounts via SSH. This is useful for my fellow developers.

Not as a developer, it is also nice that it has watchtower inside applications (all of them). Also, it actually notices when you login whether it be logging in with Google or just using a username and password. Their graphic from their website says it all:

![1PwSignInWith.png](/img/user/Digital%20Gardens/Tools/images/1PwSignInWith.png)

Also, 1Password can be used completely offline unlike Bitwarden. They state it perfectly in their FAQ:

> You don’t need internet access to use 1Password. While 1Password uses the cloud to make your data available on each of your devices, those devices maintain a local copy for fast access, so you can use 1Password offline. If you do use 1Password without an internet connection, your data will be updated to the latest version once you’re back online.

I have tested this myself and while iPadOS/iOS prompted a “you need internet connection” error on Bitwarden, in 1Password, the app is 100% usable.
## How secure is 1Password?

No one really knows except 1Password developers. This is because they are a closed source application. This means that they don’t share the back-end code with anyone except 3rd party auditors and their own developers. So, as far as anyone knows, they _could_ be as susceptible as LastPass to hacks.  
Also, I find it funny that the glitch on the image below is there. I refreshed a few times to make sure that wasn’t my browser. I even tried Edge (I use Brave, currently) and same issue. This is a display of the type of bugs I’m talking about.

![1PasswordBugs.png](/img/user/Digital%20Gardens/Tools/images/1PasswordBugs.png)

## How much does 1Password cost each year? What do you think of the pricing?

For 1 person, [1Password is $36/year and for families it is $60/year](https://1password.com/pricing). Families allow you to have up to 5 members sharing the subscription.

When you compare this pricing to Bitwarden (free or $10/year) or KeePass (free), $36/year is pretty steep for a password manager. I understand you are paying a higher price for the additional features it has over its competitors though I’m not sure how I justify the price.

Though, I have to say it is nice that 1Password is free for students via [GitHub Student Developer Pack](https://education.github.com/students). I signed up for it and confirmed with their support that while this system is made to be used once per 1Password user, you _can_ redeem yearly by setting up as a new user. Since it was [_just_ released](https://blog.1password.com/github-student-developer-pack/) on May 9, 2023 I can’t say exactly _how_ this works but I plan to find out next year since I signed up shortly thereafter. If someone can figure this out next year, please let me know. Once you sign up, your billing looks like this so you can’t really see much:

![](https://dudethatserin.com/wp-content/uploads/2023/06/image-7.png)

I had to confirm with support that I had no credit cards on file so after this plan expires next year, I will have to re-subscribe. They did confirm that if I wanted to do this without needing to export or do any glitches, I can get [50% off student discount](https://www.studentappcentre.com/App/1Password). Though that is only for 1 year as well. So it would go from Free -> 50% off -> Full Price by the time any student graduates college.

## Do you recommend 1Password? Do you use it?

Yes and Yes. 1Password is fantastic application. It is just expensive so it is hard (for me) to justify the price. Regardless of the features, there are so many bugs, support is super slow and unhelpful, and it doesn’t have that many more features than Bitwarden which is less than half the cost.

BW has a much more active support forum and while it also relies on Reddit, they also have Twitter and email support and I’ve always had good interactions with emailed support thus far though I haven’t needed them cause Bitwarden works. You can read more about it in my [[Digital Gardens/Tools/Password Managers/Bitwarden\|Bitwarden]].

---
# Other Reviews
## Articles
- [Why We Love 1Password for 2023 / Reviews by Wirecutter](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiwwf_XyMiAAxWZQzABHYNsDoQQFnoECBEQAQ&url=https%3A%2F%2Fwww.nytimes.com%2Fwirecutter%2Freviews%2F1password-review%2F&usg=AOvVaw0ARElkfZbxHbNokgKbacCn&opi=89978449)
- [1Password Review / PC Magazine](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiwwf_XyMiAAxWZQzABHYNsDoQQFnoECBAQAQ&url=https%3A%2F%2Fwww.pcmag.com%2Freviews%2Fagilebits-1password&usg=AOvVaw3hBA5T4huns7Bd8aXw1cLr&opi=89978449)
- [1Password password manager review / Tom's Guide](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiwwf_XyMiAAxWZQzABHYNsDoQQFnoECBwQAQ&url=https%3A%2F%2Fwww.tomsguide.com%2Freviews%2F1password&usg=AOvVaw3lxv8oEb7x4LkAjgh1fBjq&opi=89978449)
- [1Password Review - Cloudwards](https://www.cloudwards.net/1password-review/)
- [1Password Software Reviews, Pros & Cons - Software Advice](https://www.softwareadvice.com/encryption/1password-profile/reviews/)
- [1Password Review - Tech.co](https://tech.co/password-managers/1password-review)
## YouTube Videos
These are all embedded, open the callouts to show the videos and you can watch them right here on our site.

> [!info-darkbg]- 1Password Review & Tutorial - CyberNews
> <iframe width="560" height="315" src="https://www.youtube.com/embed/RsVL-qloXq8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-darkb]- Is 1Password Safe in 2023 - CyberNews
> <iframe width="560" height="315" src="https://www.youtube.com/embed/9pROgt9jdYQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-darkg]- 1Password Review | My thoughts after 1 year of use (Pros vs Cons) - All Things Secured
> <iframe width="560" height="315" src="https://www.youtube.com/embed/fYuzFSuVREw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-darko]- 1Password Walkthrough - All Things Secured
> <iframe width="560" height="315" src="https://www.youtube.com/embed/_lw8_6wupkY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-lighty]- 1Password vs Bitwarden Honest Review - CyberNews
> <iframe width="560" height="315" src="https://www.youtube.com/embed/PE0aIdXE8oY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-lightpp]- Best Password Manager 2023 - Ultimate Comparison - Pete Matheson
> <iframe width="560" height="315" src="https://www.youtube.com/embed/99P59LS1rrw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

> [!info-lightdb]- STOP Using Your Password Manager NOW! - Pete Matheson
> <iframe width="560" height="315" src="https://www.youtube.com/embed/oZzisbY7fYs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

