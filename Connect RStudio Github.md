# How to connect RStudio with Github?
Here, we'll discuss the process to connect your desktop RStudio with Github, so that you can manage all your R codes in global/remote from your local machine.
You all are pretty familiar with Github. So, I'll not discuss about Git or Github here, if you want to know details, you can [follow tutorials](https://www.youtube.com/watch?v=SWYqp7iY_Tc) and do some reasearch online.

You need to have three items available to get this service
* R and RStudio in your desktop (Download [R](https://cran.r-project.org/bin/windows/base/), [RStudio](https://www.rstudio.com/products/rstudio/download/) and install it)
* Git in your desktop (Download [Git](https://git-scm.com/downloads), and install it)
* A [Github](https://github.com/) account

Once you are done with all of those three items, you can proceed to your local work to global/remote.

## Step One: Authentication
You need to take a authintication token to get access to Github from you local RStudio. You need to sign in your Github account and follow the corresponding steps-

**[Github](https://github.com/) account** > **Settings** > **Developer settings** > **Personal access tokens** > **Generate new token** > **Add note, select expiration, tick repo section** > **Generate token**

![Screenshot1](https://www.dropbox.com/s/s9nn85o0m12skqh/C1.png?dl=0)
