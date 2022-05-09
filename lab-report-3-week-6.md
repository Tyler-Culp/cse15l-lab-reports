# Streamlining ssh Configuration
![pic1](Lab3SS_1.png)
The first thing I did to steamline the ssh process is to create a config file. I created and edited this file just through my terminal on my mac.

The screenshot below shows me logging into the server using just `ssh ieng6`. 
![pic2](LabReport3SS_2*.png)

In this next screenshot you can also see how much easier it is to scp files now that tis config file is set up. Now I only need to do `scp [filename] ieng6` to copy files over to the server. The screenshot below shows me doing this.

![pic3](Lab3SS_3*.png)

# Setup Github Access from ieng6

Now we will look at ssh keys added to github. Below shows where the key is stored for me on github:
![pic4](Lab3SS_4*.png)

And this shows me commiting and pushing my changes to github from my terminal:

![pic5](Lab3SS_5*.png)

and here is the [link](https://github.com/Tyler-Culp/cse15l-lab-reports/commit/f4243d1f70d35178594238009d671dcd834ba83c) for the last commit.

# Copy whole directories with scp -r

We can copy over whole directories to our ieng6 accounts with scp by using `scp -r . cs15lsp22apz@ieng6.ucsd.edu:~/[directory_name]` as shown below using the markdownParser directory:
![pic6](Lab3SS_6*.png)

The next screenshot shows me accessing my ssh account and going into the markdownParser directory that is now there, and then running my JUnit tests from the ieng6 account:

![pic7](Lab3SS_7*.png)

Finally this last screen shot shows me combining scp with ssh to be able to copy the directory and run a test with markdownparser all on a single line.

![pic8](Lab3SS_8*.png)

