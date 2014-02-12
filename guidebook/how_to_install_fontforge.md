<h1>How To Install FontForge</h1>

<p>This page is step by step guide to installing <a title="FontForge" href="/wiki/FontForge">FontForge</a> for beginners.</p>

<h4> Windows </h4>

Please see this guide on how to <a href="http://www.mpetroff.net/software/fontforge-windows/">install FontForge on Windows</a>.</p>

<h4> Mac OS X </h4>

Please see this guide on how to <a href="http://www.pixilate.com/about/installing-fontforge-in-mountain-lion">install FontForge on Mac OS X</a>. (To solve copy-paste problems with FontForge and also Inkscape, change the X11 preferences' "Pasteboard" settings to that "Enable syncing" is disabled.)</p>

<h4> GNU/Linux </h4>
<a id="Install_the_required_programs" name="Install_the_required_programs"></a><h4> <span class="mw-headline"> Install the required programs </span></h4>

<p>The parts in the light blue boxes are commands that should be typed (copy and pasted) into your "Terminal" program.</p>

<p>When using Debian or Ubuntu:</p>

<tt>sudo apt-get update; sudo apt-get install -y autoconf libtool libpng12-dev zlibc zlib1g-dev libtiff-dev libungif4-dev libjpeg-dev libxml2-dev libuninameslist-dev xorg-dev subversion cvs gettext git libpango1.0-dev libcairo2-dev python-dev uuid-dev  libreadline-dev libltdl-dev;</tt>

<p>and enter your password when prompted.</p>

<p>When using Fedora or Red Hat:</p>
<tt>
   sudo yum update;
   sudo yum install -y libpng-devel zlib-devel libtiff-devel giflib-devel 
   libjpeg-devel libxml2-devel libuninameslist-devel cairo-devel 
   python-devel cvs git subversion mercurial pango-devel 
   libtool-ltdl-devel libtool-ltdl libtool libuuid-devel readline-devel czmq-devel; 
   sudo yum groupinstall -y x-software-development development-tools;
</tt>

<p>and enter the root password when prompted.</p>

<a id="Download_FontForge_dependencies" name="Download_FontForge_dependencies"></a><h4> <span class="mw-headline"> Download, Compile and Install FontForge Dependencies </span></h4>

<p>First, use the 'change directory' command "cd" to ensure you are in your 'home directory' ("~"). Then make a "source code" folder with the 'make directory' command "mkdir" to keep things tidy. Then change to that directory.</p>

<tt>   cd ~;
   mkdir src;
   cd src;
</tt>

<p>Using the Git version control program, download the other source code to enable all of FontForge's features: Freetype2 is a text rendering system used to draw fonts on screen; libspiro is the Spiro drawing program that is integrated into FontForge; libuninameslist is a program for looking up descriptions of unicode characters, and libzmq and czmq are programs required for the new real time collaboration feature.</p>

<tt>
   git clone git://git.sv.gnu.org/freetype/freetype2.git;
   git clone https://github.com/fontforge/libspiro.git;
   git clone https://github.com/fontforge/libuninameslist.git;
   git clone https://github.com/zeromq/libzmq.git;
   git clone https://github.com/zeromq/czmq.git;
</tt>

<p>These 3 commands change to the libspiro directory, configure, compile and install it:</p>

<pre>
autoreconf -i; # you might be able to try autoconf
automake;
./configure;
make -j 4 -k;
make check;
sudo make install;
</pre>

<p>These 3 commands change to the libuninameslist directory, configure, compile and install it:</p>

<pre>   cd ~/src/libuninameslist; ./configure; make -j 4 -k; sudo make install;</pre>

<p>These 3 commands change to the libzmq directory, configure, compile and install it:</p>

<pre>   cd ~/src/libzmq; ./autogen.sh; ./configure; make -j 4 -k; sudo make install;</pre>

<p>These 3 commands change to the czmq directory, configure, compile and install it:</p>

<pre>   cd ~/src/czmq; ./autogen.sh; ./configure; make -j 4 -k; sudo make install;</pre>

<a id="Download_FontForge_source_code" name="Download_FontForge_source_code"></a><h4> <span class="mw-headline"> Download FontForge source code </span></h4>

<p>Typically, you will want to download the latest daily source code, with the "git" version control system, hosted by the GitHub website. To do this, run:</p>

<tt>cd ~/src/; git clone https://github.com/fontforge/fontforge.git;</tt>

<a id="Compile.2C_install_and_run_FontForge" name="Compile.2C_install_and_run_FontForge"></a><h4> <span class="mw-headline"> Compile, install and run FontForge </span></h4>

<p>Now configure, compile and install FontForge:</p>

<tt>   cd ~/src/fontforge/;
    ./bootstrap;
   ./configure --with-freetype=../freetype2;
   make -j 4 -k;   
   sudo make install;
   sudo ldconfig;
</tt>

<p>Finally, run FontForge:</p>

<pre>   /usr/local/bin/fontforge;</pre>

<h4> Updating your source code </h4>

<p>You don't have to do all this each time you want to update. Just run the following commands:
</p>
<tt>   cd ~/src/libspiro; make clean; svn up; ./configure; make; sudo make install;
   cd ~/src/freetype2; git pull;
   cd ~/src/fontforge; git reset --hard; git pull;
   ./bootstrap; ./configure --with-freetype=../freetype2;
   make -j 4 -k; sudo make install; sudo ldconfig;
</tt>
