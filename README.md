# image-classifier-star-wars-
This is an image classifier using Tensorflow and python

- Please refer to this video for the tutorial https://youtu.be/QfNvhPx5Px8.  Credits to Siraj for this tutorial and challenge.
- You can also refer to this link to help with the tutorial, as mentioned by Siraj: https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/?utm_campaign=chrome_series_machinelearning_063016&utm_source=gdev&utm_medium=yt-desc&authuser=1#0
- You may also refer to another git hub repository that helps explain steps in building this image classifier: github.com/hiteshvaidya/Star-wars-classifier
- This repository was built to explain my process since I continuted to face difficulties aside from the help attained by the sources mentioned above.  This classifier was built using Windows 8.1 standard edition.  

The star wars image classifier is explained and executed in 7 steps.  The steps taken by me differ a bit to work with the windows 8.1 system since I encountered errors and I want to note that I am beginner to Tensorflow.

Step 1) Install Docker - To install docker you'll need to ensure that you have visualization enabled on your computer; the requirements for Docker are explained on the Docker site.  You can check this by going to your task manager and click the tab 'Performance' and near the botton right corner you should see 'Visualization.'  If it shows disabled then you need to go through the BIOS to enable it.  Since I'm using windows 8.1 standard, the Hyper-V client does not come with the machine, therefore the Docker Toolbox will need to be installed.  It contains everything necessary, including the Oracle VM virtual box. Note: If you have a windows version that contains Hyper-V, once visualization is enabled or if already enabled, check to see if you have Hyper-V enabled.  To do this, you may follow this tutorial - https://blogs.technet.microsoft.com/canitpro/2014/03/10/step-by-step-enabling-hyper-v-for-use-on-windows-8-1/

Step 2) Install the TensorFlow Image on the Docker VM - Type the code as mentioned and shown by Siraj in the tutorial.  Once you see the '#' you'll know it is complete and that you have installed the TF image.

Step 3) Download the dataset - You'll need to download two datasets - one for Darth Vader and the other for Darth Maul - to be able to compare to each other for your image classifier.  Downloading and using the google add-in Fatkun helps, as mentioned in the video.  Once you've made your image directory, you can move your image datasets to the directory.  Since I had trouble in the future steps with linking my image directory with TF, I decided to create a folder tf_files, and two more folders (not just one as mentioned in the video and I'll explain why): star_wars and star_wars2.  The star_wars folder was created in order to store the folders that would be created in step 7 as well as my python script, and star_wars2 is used as the image directory. Note that I placed star_wars2 in the star_wars folder because of step 4.  After I continued to encounter issues in step 4 with linking, I decided created two folders in step 3 would solve the issue and it did. To move your image folders (named 'darth vader' and 'darth maul'), first cd into the folder where you want to store the images, in my case is used cd /tf_files/star_wars/star_wars2/ Once you are in the folder I moved my image folders using: 
mv $HOME/Downloads/darth\ vader . - You should then see the darth vader folder in your star_wars2 folder.  Enure you have a spacebar then {.} after \ vader. 

Step 4) Linking the Tensorflow image to the dataset - the method used in the tutorial did not work for me.  I created the folders as mentioned in the tutorial, however I noticed upon linking that the tf_files folder was not visible and only the star_wars folder was visible.  I also noticed that by checking the contents of the star_wars folder, the image folders 'darth vader'and 'darth maul' were not visible.
