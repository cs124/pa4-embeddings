# PA4 - Embeddings

## Recommended before Starting

We recommend checking out the following before getting started on PA4:

* The Week 5 videos and slides on Canvas.
* The J+M readings on Vector Semantics and Embeddings

## Cloning the Assignment

### Jupyter Notebook

You can get started using the same steps you followed for PA1-3. To recap,
you'll want to:

1. Open a terminal (terminal for macOS and Linux, 
   Ubuntu for Windows for Windows, or SSH into Rice/Myth) the same way you 
   did for PA0. 

1. Clone the git repository for PA4 (this repository) into a folder of your 
   choice by typing this in your terminal:
      
        git clone https://github.com/cs124/pa4-embeddings.git

2. Enter the project root directory:
   
        cd pa4-embeddings

3. Activate your environment. This assignment requires additional packages that you need to install! You have two options:

   - If you want to installed required packages into your cs124 environment, run:
   
         conda activate cs124
         conda install -c pytorch pytorch
         conda install -c huggingface transformers
   
   - If the option above doesn't work for you, or you prefer to create a new environment, run:
   
         conda env create -f environment_pa4.yml
         conda activate cs124_pa4

   You'll need to activate your environment every time you open a new terminal and re-start your
   notebook server.

3. Start up your jupyter notebook server

        jupyter notebook

4. A window should open automatically in your default browser. If it didn't,
    the terminal output should contain a URL you can use to open the
    notebook in a browser of your choice.
   
5. From the Jupyter notebook file explorer window that opens, click on the
pa4.ipynb file to open and edit it.

### Google Colaboratory

1. Go to [colab.research.google.com](http://colab.research.google.com). 
   If prompted to open a notebook, hit cancel for now. You should double-check 
   that you are logged in to your Stanford Google account. If not, you can 
   switch accounts in the top right.
   
2. Now go to File->Open Notebook. Go to the GitHub tab. It will ask you to log 
   in to your GitHub account (if you don't have one it is easy to make one).
   Once you've done that, copy and paste the URL: 
   https://github.com/cs124/pa4-embeddings into the search box and hit enter. 
   It should show:
   
            Repository: cs124/pa4-embeddings
            Branch:  Main

   Click on pa4.ipynb below to load the notebook.
      

## Submitting your Solution

### macOS/Linux

1. You can run the submission cell in the Jupyter notebook to zip up your
solution for you. It should generate a zip file `submission.zip`.
   
2. Upload the zip file as your solution to the PA4 Embeddings assignment in 
   Gradescope (http://www.gradescope.com).

### Ubuntu for Windows

1. You can run the cell at the bottom of the Jupyter notebook to zip up your
solution for you. It should generate a zip file `submission.zip`.
   
2. Run the following command to transfer that zip file over from WSL to your local computer:

      cp ~/cs124/pa4-embeddings/submission.zip /mnt/c/Users/YOUR_USER_NAME/OneDrive/Desktop/

   Note that you may want to replace OneDrive/Desktop/ with another destination folder based on your preferences.

3. Upload the zip file as your solution to the PA4 Embeddings assignment in 
   Gradescope (http://www.gradescope.com).

### Rice/Myth

1. You can run the cell at the bottom of the Jupyter notebook to zip up your
solution for you. It should generate a zip file `submission.zip`.
   
2. You will then need to download/copy the zip file from Rice/Myth to your
local machine.
   
   - __[macOS/Linux/Ubuntu for Windows]__
    
      After you have created the submission zip, cd into a local folder where you'd like to copy the submission zip from Myth, and use the following command to copy the zip from Myth to your local machine:

         scp -r [SUNet]@[rice/myth].stanford.edu:/path-to-your-pa4-folder/submission.zip .
      
      You can replace . with a relative path to a local directory you'd like to copy the zip file to.

   - __[Windows]__ PSCP is another utility that should have been installed
    automatically when you installed PuTTY earlier. Find and run it. In the
     terminal window, you can run the command:
     
            pscp [Your SUNet]@rice.stanford.edu:/path/to/submission.zip c:\temp\submission.zip
    
    to download the file from Rice/Myth to your local machine. You should now
   be able to access the file locally at c:\temp\submission.zip
   
3. Upload the zip file as your solution to the PA4 Embeddings assignment in 
   Gradescope (http://www.gradescope.com).

### Google Colaboratory

1. Once you've saved all your changes, go to File->Download .ipynb to download
your notebook file to your local machine.
2. If your solution required any extra files, make sure they were located in
pa4-embeddings/deps. Go to the file explorer on the left-hand side and download
those as well.
3. Once you have pa4.ipynb and any deps files you need saved locally,
create a zip file (either from your OS's file explorer or the terminal), making
sure that it has the following structure:
   
        deps/
        pa4.ipynb

3. Upload the zip file as your solution to the PA4 Embeddings assignment in 
   Gradescope (http://www.gradescope.com).
