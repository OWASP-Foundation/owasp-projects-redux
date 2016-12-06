# DRAFT VERSION

## Transfering your existing Github repository into the OWASP Github organization

Below are the steps required to get an existing repo listed in the OWASP Github organization

### Prerequisites

* An active OWASP project whose code/content is in a public Github repo
* An account on OWASP's Slack 
  * If not, register your email address [here](http://owasp.herokuapp.com/)

#### Known issues

* Heavily integrated projects will have some of those integrations break and will need some reconfiguring/fixing
* Reported working integrations
  * [Travis CI](https://travis-ci.org/)
  * Github Stars, Forks, Watches, Collaborators...
* Reported failing integrations
  * [HuBoard](https://huboard.com/) - reported to have a 'Fix All' button for this situation
  * [Gemnasium](https://gemnasium.com/)
  * [DockerHub](https://hub.docker.com/)
* Untested/unknown integrations
  * [Heroku](https://www.heroku.com/)
  * [Gitter.im](https://gitter.im/)
  * [Wakatime](https://wakatime.com/)
  * [Nodesecurity.io](https://nodesecurity.io/)
  * [Appveyor](https://www.appveyor.com/)
  * [Versioneye](https://www.versioneye.com/)
  * [Amazon SNS](https://aws.amazon.com/sns/)
  * [Codeclimate](https://codeclimate.com/)
  * [Bountysource](https://www.bountysource.com/)
* For older SSH keys, you may see an error when you git push.
  * See "SSH Key workaround" at the bottom of this document

### Transfering to OWASP's Github Organization

1. Setup a time with OWASP staff to meet on Slack
  1. Use the [Contact Us](https://www.tfaforms.com/308703) form and select _"IT Support"_ for the "I need help with" dropdown list
  1. Please use the following in the description
    1. The name of your OWASP project
    1. A couple of times you are free and your timezone e.g. GMT-6
    1. Your Github username
    1. The name of your Github repo to transfer
    1. The URL of your Github repo
1. OWASP staff will contact you to confirm the time to meet on Slack
1. During the Slack meeting
  1. You'll be asked to go to the settings for the repo you want to transfrer
  1. Once on the repo settings page, wait for OWASP to tell you that its ready to accept your repo into the OWASP Github org
  1. Do the transfer when instructed
  1. OWASP staff will let you know the transfer is complete.
1. Enjoy your **_new found fame_**

See [Github's Help](https://help.github.com/articles/transferring-a-repository-owned-by-your-personal-account/#transferring-to-an-organization) for more information on transfering repos to an organization

### Visual version of transfering a repo to OWASP's Github org


Log into Github and go to your profile page

![OWASP Github Transfer - image 01](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-01.png "Go to your profile page on Github")

During the Slack meeting, you'll get an email inviting you to the OWASP org

![OWASP Github Transfer - image 02](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-02.png "Email invite to the OWASP Github org")

Clikcing on that link will take you to Github's invitation page

![OWASP Github Transfer - image 03](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-03.png "Github page inviting you to the OWASP org")

After you accept the invitiation, you'll be forwarded to the OWASP org page

![OWASP Github Transfer - image 04](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-04.png "Github page welcoming you to the OWASP org")

Browse (or re-browse) to the repo you are transfering

![OWASP Github Transfer - image 05](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-05.png "Go to the repo you are transfering")

Click on the settings tab and scroll to the bottom to the **"Danger Zone"** - do not click "Transfer" yet

![OWASP Github Transfer - image 06](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-06.png "Under the settings tab, scroll to the Danger Zone - no clicking yet")

Once OWASP staff says things are ready, click on "Transfer" and fill out the window that opens

![OWASP Github Transfer - image 07](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-07.png "Click Transfer and fill out the window that pops up")

You will be forwaded to a page about Team access, just click "Transfer" - you can always do team creation, membership, etc in the future.

![OWASP Github Transfer - image 08](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/owasp-github-transfer-08.png "You can skip Team access for now")

That's it, your repo will now be part of the OWASP Github org.  **Congrats!**

### SSH Key Workaround

If you get an error message like:

```
ERROR: Sorry, but @OWASP has blocked access to SSH keys created by some third-party applications. Your key was created before GitHub tracked keys created by applications, so we need your help.

If you personally created this key, you can approve it at:

  https://github.com/settings/ssh/audit/123456/policy

Otherwise, please upload a new key:

  https://github.com/settings/ssh

Fingerprint: 15:axxxxxxxx:64

[EPOLICYKEYAGE]

fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

You will need to follow that link (log into Github if not already) and approve the key.  Following that link, you'll see a web page similar to the one below:

![Approve SSH Key](https://github.com/OWASP/owasp-projects-redux/raw/master/github-org/images/ssh-key-approve.png "Approve your previous SSH key if you uploaded it")



