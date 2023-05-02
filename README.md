Download Link: https://assignmentchef.com/product/solved-cop4600-ex1-the-command-line
<br>
<h2>Overview</h2>

You will learn about Linux terminal commands that will greatly help you in this class. If you are an experienced user in terminal commands or command line navigation, this exercise will just serve as a refresher. You will take a screenshot of some commands that you use, and you will also submit a tar file to Canvas for this assignment.

<h2>File Packaging</h2>

There are many times that you will find yourself needing to package or compress (or unpackage and uncompress) files while working on projects. <strong>TAR </strong>(originally Tape Archive – packs / creates an archive) and <strong>Gzip </strong>(GNU zip) are two commonly used tools in Unix based operating systems. To familiarize yourself with these commands and how they work, complete the following and take a screenshot:




<ul>

 <li>Create a file (e.g., “somefile.txt”) using a text editor (e.g. <strong>nano</strong>)</li>

 <li>Use <strong>gzip</strong> to compress the file, yielding a gzipped file (“somefile.txt.gz”)</li>

 <li>Use <strong>gunzip</strong> to decompress the file, yielding the original file (“somefile.txt”)</li>

 <li>Create a second file (“other.txt”)</li>

 <li><strong>Create an archive</strong> from <strong>both files</strong> (“somefile.txt” &amp; “other.txt”), yielding “myfiles.tar” (<strong>tar -cvf</strong>)</li>

 <li><strong>Extract the files</strong> from the archive (<strong>tar -xvf</strong>)</li>

 <li>Create a new file (“somefile2.txt”)</li>

 <li>Create an archive file from all <strong>three text files</strong> piped through gzip to create a “.tar.gz” (<strong>tar -zcvf</strong>)</li>

 <li>Type “<strong>ls</strong>” to view the current directory and your “.tar.gz”</li>

 <li><strong>Unzip and Extract</strong> the “.tar.gz” (<strong>tar -xzvf</strong>)</li>

 <li>Type “<strong>ls</strong>” to view the current directory and your extracted file.</li>

 <li>Take a screenshot of the commands run in steps 7) through 11).</li>

</ul>




Once finished you should have extracted readable content from the “.tar.gz”. You will use these tools to package and compress files that you will submit for projects, so make sure you understand how they work!

<h2>Terminal Navigation</h2>

The navigation exercise can be completed by following these steps, including taking two screenshots (see step 4):




<ul>

 <li>Create a folder with the name format <em>last_first</em> (e.g., “<strong>sanchez_richard</strong>”) in <strong>/home/reptilian</strong>.</li>

 <li>Issue a command to find files that contain the phrase “<strong>android_dev</strong>” from the kernel source directory.</li>

 <li>Reissue the command from (2); this time, pipe the output of the command to a text file named “<strong>txt</strong>”. 4) Take a screenshot of the command in 3) and another with a listing of the directory of the first file from 2). 5) Move or copy “<strong>ex1.txt</strong>” into the directory created in (1).</li>

 <li>From <strong>/home/reptilian</strong>, create a tar file named <strong>tar</strong> of the directory from (1) (including contents).</li>

 <li>Use <strong>gzip</strong> to compress <strong>tar</strong> (yielding <strong>ex1.tar.gz</strong>).</li>

 <li>Create “<strong>7</strong>”, describing steps 1-7, using a text editor (e.g. <strong>nano</strong>). <em>(See </em><a href="https://liw.fi/manpages/"><em>https://liw.fi/manpages/</em></a><a href="https://liw.fi/manpages/"><em>)</em></a> 9) From your local command line, use <strong>sftp</strong> to transfer the files created in (7) and (8) back to your local host.</li>

</ul>

10) Submit <strong>ex1.tar.gz</strong>, <strong>ex1.7</strong>, and your three screenshots on Canvas.

<h2>Package Installation</h2>

Sometimes you’ll need to install new packages from within a Linux system. On Debian-derived distributions, you can use the <strong>apt</strong> command for this. Here an example to install the <strong>man</strong> utility:




<strong>$</strong> <strong>sudo apt install man</strong>




Once installed, you can use <strong>man</strong> to view manual pages.

<h2>File Transfer</h2>

You will need to use the local Unix shell (on Windows, via WSL or MSYS) to execute the sftp command in order to transfer files from the virtual machine to the local host:




<strong>$</strong> <strong>sftp <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="ed9f889d998481848c83addcd4dfc3dcdbd5c3dcc3dcdedd">[email protected]</a></strong><strong>        </strong>Replace with VM IP address




Once connected, you can issue the “help” command from within <strong>sftp</strong> for more information