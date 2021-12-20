# How to connect RStudio with Github?
Here, we'll discuss the process to connect your desktop RStudio with Github, so that you can manage all your R codes in global/remote from your local machine.
You all are pretty familiar with Github. So, I'll not discuss about Git or Github here, if you want to know details, you can [follow tutorials](https://www.youtube.com/watch?v=SWYqp7iY_Tc) and do some reasearch online.

You need to have three items available to get this service
* R and RStudio in your desktop (Download [R](https://cran.r-project.org/bin/windows/base/), [RStudio](https://www.rstudio.com/products/rstudio/download/) and install it)
* Git in your desktop (Download [Git](https://git-scm.com/downloads), and install it)
* A [Github](https://github.com/) account

Once you are done with all of those three items, you can proceed to your local work to global/remote.

## Step One: Authentication
You need to take a authentication token to get access to Github from you local RStudio. You need to sign in your Github account and follow the corresponding steps-

**[Github](https://github.com/) account** > **Settings** > **Developer settings** > **Personal access tokens** > **Generate new token** > **Add note, select expiration, tick repo section** > **Generate token**

![Authentication process](C1.png)
![](C2.png)

**Note: Don't forget to copy & save the access token to a notepad.** Because once you refresh your browser, you won't get the code again.

## Step two: Setup RStudio
#### Check RStudio
Once you have the access token, now it's time to setup your RStudio. Before you start for the setup, you need to check that you RStudion is enable for version contron interface for projects or not. Follow the corresponding steps to check this.

**RStudio** > **Tools** > **Global Options** > **Git/SVN** > **Tick** Enable version control interface for RStudio projects > **Apply**
![](C3.png)

#### Create a project
You need to create a project that you want to work with and store it to Github. In this step, you need to go with this following steps-

**RStudio** > **File** > **New Project** > **New Directory** > **New Project** > Put a **Directory name** & **tick on** Create a git repository > **Create Project**
![](C4.png)

#### Edit environment and start your project
In the previous step we've created the project. Now, it's time to start the project with our project task. Let's create a R script, say **Test.R** and install the library **usehis**. So, we need to run the below codes in the console or in your script

``
install.packages("usethis")

library(usethis)

edit_r_environ()
``
