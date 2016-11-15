# project-transcribe-a-card

This is the template for the Transcribe-a-Card projects seen on LibCrowds.


## Workflow

The workflow established for Transcribe-a-Card projects is as follows:

#### 1. Create a new project

1. Create a [new project](http://www.libcrowds.com/project/new).
    - The suggested format for the name is *Transcribe Language*.
    - The suggested format for the short name is *transcribe_language*.
    - Enter any text into the long description field, it will be replaced automatically during the next few steps.
2. Select Dashboard from the side menu then Sync with GitHub.
3. Enter the URL of this page (https://github.com/LibCrowds/project-transcribe-a-card) and click Continue.
4. Scroll to the bottom of the following page and click Update.
5. Select Dashboard from the side menu then Import Tasks.
6. Select the Flickr importer and, if necessary, log in using the LibCrowds Flickr credentials.
7. Select your album and click Import.
    - **Important:** If importing a large number of tasks, wait for the email to
    let you know that the import has finished before proceeding.
8. Once all tasks are imported, from the Dashboard click Task Redundancy.
9. Enter **3** and click Set Redundancy.
10. To publish the project visit the Dashboard again and click Publish.

**Note:** The steps above describe how to create a new project using
[pybossa-github-builder](https://github.com/alexandermendes/pybossa-github-builder).
There are various other ways to create new projects, all of which are
described in the [PyBossa documentation](http://docs.pybossa.com/en/latest/user/overview.html).


#### 2. Analyse the results

For all tasks where two contributors submitted exactly the same answer the
final result will automatically be set to that answer. For all other tasks human
intervention will be required to determine which answer should be accepted.

1. Sign in and select Open Project from the menu at the top right of the screen. Here
   you will see all projects for which you are the project owner.
2. Open the project then from the left-hand menu click Analysis. If there are tasks pending analysis you will
   be presented with a card and all associated answers. Otherwise, a message will be displayed
   saying that there are no unanalysed results to process.
    - When you first visit the analysis application you'll be asked for a username and password, which can
      be supplied by a LibCrowds administrator.
    - Users other than the project owner can also help analyse results by visiting the following URL directly: `https://analyse.libcrowds.com/<project_short_name>`
3. Use the radio buttons to select the correct answers. You can also enter your own answer by clicking on the
   radio button next to the blank text field and entering the relevant text.
4. To spot check results open the project as in steps 1 & 2 and select Results from the side menu.

**Important:** Once a project has been completed ensure that all results are analysed by either clicking through
to the analysis application, as in step 3, or by downloading the relevant CSV file from the [LibCrowds Data](https://www.libcrowds.com/data/) page
and ensuring that there are no rows with 'Unanalysed' in the *info* column.


#### 3. Submit the data

Metadata services will handle the transformation of records. Once all results have been analysed either download the XML file from the
[LibCrowds Data](http://www.libcrowds.com/data) page and send it over, or just let them know which project has been completed so that
they can pull the data themselves.

**Important:** If any changes are subsequently made, for example, if certain records are not able to be
ingested, the associated results should be updated on the system by visiting
`https://analyse.libcrowds.com/<project_short_name>/<result-id>`. This ensures that we can later
identify the cards that still need to be processed by alternative means. The result ID can be found
in the results CSV file.


## Uploading images to Flickr

Below are some basic guidelines for uploading images to Flickr, for further help
please refer to the Flickr documentation.

1. Log in to [Flickr](https://www.flickr.com) using the LibCrowds credentials.
2. Click the upload icon at the top right of the screen.
3. Select your images.
    - **Important:** Wait until all images have loaded before proceeding! To check,
    scroll to the bottom of the window and wait for the thumbnails to appear.
4. Click All on the toolbar to select all images.
5. Click **Add to albums** and create a new album for **this specific LibCrowds project**.
6. Click **Upload n Photos** at the top right of the screen.


## Downloading images

The analysis application can be used to download sets of images from Flickr by listing their
task IDs in the form at `https://analyse.libcrowds.com/<project_short_name>/download`. You can
visit this URL by clicking the Download Input menu link in your project dashboard. The
task IDs can be found in the results CSV file for your project. These task IDs can be found
in the results CSV file.
