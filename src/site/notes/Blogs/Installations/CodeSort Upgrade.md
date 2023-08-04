---
{"dg-publish":true,"dg-created":"2023-06-09T17:15:33Z","dg-updated":"2023-06-09T17:46:25Z","tags":["software","web","affiliate buttons","affiliates","buttons","collective","collection","affies","sort","codesort","codes","code"],"title":"CodeSort Upgrade","meta-tags":{"og:title":"CodeSort Upgrade","description":"CodeSort is a simple PHP script that saves affilaite buttons for your users to use to link back to your site. This is a popular software with the fanlisting community and I wrote how you can upgrade from version 2 to version 1.0 from Robotess for PHP 7.4.","og:image":"https://dudethatserin.com/-Attachments/UOB3h5M9pL.png"},"permalink":"/blogs/installations/code-sort-upgrade/","dgPassFrontmatter":true,"created":"2023-06-09T17:15:33Z","updated":"2023-06-09T17:46:25Z"}
---

CodeSort is a way to sort through your affiliate buttons for your website. This is a popular thing in the fanlisting community. If you don't know what a fanlisting is, I go over it in my [[Blogs/Installations/Listing Admin Upgrade\|Listing Admin Upgrade]] article. I will copy the basic quote over though:
> A fanlisting is simply an online list of fans of a subject, such as a TV show, actor, or musician, that is created by an individual and open for fans from around the world to join. There are no costs, and the only requirements to join a fanlisting are your name and country. Fanlistings do not have to be large sites (although some are); they are just a place where you can sign up with other fans. TheFanlistings.org is the original (but not official) web directory for fanlistings, dedicated to uniting the fans.

Let's get into the steps so you can upgrade yourself from version 2 to Robotess' Version 1.0!
# Step 1 - Make sure you have the correct PHP version installed
You may need to contact your hosting provider to check. You want to make sure your PHP version is on 7.4. Anything higher is not supported as of the date of this writing. Anything lower and you will need an older fork and it is not recommended as newer versions of software protect you from hacks and losing data.
# Step 2 - Backup your files
You want to make sure you have them backed up in case anything happens to your files.
# Step 3 - Make sure you have CodeSort version 2 installed
*Note:* If you already have CodeSort installed (any version) you will want to make sure you are updated to (at least) version 2. You can do that with the files I have linked below. Once you are on version 2+, you are good to continue with step 4.

This is the next step as you cannot *upgrade* without first having an older version installed. If you do not have it installed I have a repository of all of the downloads [here](https://github.com/DudeThatsErin/downloads). You will want to click on `codesort.zip` and then `view raw` and that will prompt a download. Just download it, extract it and upload the contents (all of them) to your website.
Once you have it uploaded you **do not**, I repeat, **do not** need to install it. You just need to make sure that `https://yourdomain.com/codesort/codesort2/install.php` shows up and you see weird errors that say something about `T_NEW` errors. If that is the case, you are good to continue.
# Step 4 - Download Robotess' Files
I have links to everywhere you can get updated files [here](https://github.com/DudeThatsErin/downloads/tree/main/updated-files) here link though is [here](https://scripts.robotess.net/). You will want to visit that website & click  on `Projects` at the top. Then you will want to click on `CodeSort for PHP 7` which should have a link to her gitlab. Click on that or [click here](https://gitlab.com/tfl-php-scripts/codesort).

Once you get there, scroll down and read the `README.md` or [click this link](https://gitlab.com/tfl-php-scripts/codesort/-/archive/master/codesort-master.zip?path=codesort2) to download a repo of the updated files. You will want to extract those and upload them to your website.
# Step 5 - Upload them to your website
Once you have them extracted, you will want to **overwrite** all of the files that are on your site. It is **highly recommended** to take a backup of your files first before doing this (in case something goes wrong).
Once you have the backup and have everything overwritten. Visit `https://yourdomain.com/codesortinstall/install.php` and it should look show errors like this:
![codesort-err.png](/img/user/Blogs/-Attachments/codesort-err.png)
That is fine. You just need to update your `codes-config.php` file. Open that file in your editor and find these lines:
```php 
// ------------->ADMIN VARIABLES

$codesort['admin_username']	= 'admin';
$codesort['admin_password']	= md5('pass');

// ------------->DATABASE VARIABLES

$codesort['dbhost']		= 'localhost';
$codesort['dbuser']		= 'username';
$codesort['dbpass']		= 'password';
$codesort['dbname']		= 'database';

// ------------->TABLE VARIABLES

// Which script do you use for your fanlistings collective?
// Currently, the supported options are:

// Enthusiast			'e'
// Flinx Collective		'f'
// Fan Admin			'g'

// Or if you don't use one, enter 'n'

$codesort['collective_script']	= 'e';
```
They should go from line 25 to line 48. Starting at the top, you will want to change your login details. It is **highly recommended** you **never** use `admin` for a username. So change both of those.
Then you will want to update the database variables to your database information. You can use your existing fanlisting collective database or use a new database.
If you are using this in combination with a fanlisting collective select the version you have. If you don't use any of those 3 options, change the `e` to an `n`.
Save and close the file. Reload (or visit) your install file again and it should look like so:
![UOB3h5M9pL.png](/img/user/Blogs/-Attachments/UOB3h5M9pL.png)
Fill out all of the information and click on `Create Fresh Installation` and it should install successfully.

Go to the login page at `index.php` to verify. Then **delete** the `install.php` file from your server and you are good to go!