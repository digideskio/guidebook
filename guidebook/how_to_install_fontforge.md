<h1>How To Install FontForge</h1>

<p>This page is step by step guide to installing <a title="FontForge" href="/wiki/FontForge">FontForge</a> for beginners.</p>

<h4> Windows </h4>

Please see this guide on how to <a href="http://www.mpetroff.net/software/fontforge-windows/">install FontForge on Windows</a>.</p>

<h4> Mac OS X </h4>

Please see this guide on how to <a href="http://www.pixilate.com/about/installing-fontforge-in-mountain-lion">install FontForge on Mac OS X</a>.</p>

<p>(To solve copy-paste problems with FontForge and also Inkscape, change the X11 preferences' "Pasteboard" settings to that "Enable syncing" is disabled.)</p>

<h4> GNU/Linux </h4>
<a id="Install_the_required_programs" name="Install_the_required_programs"></a><h4> <span class="mw-headline"> Install the required programs </span></h4>
<p>The parts in the light blue boxes are commands that should be typed (copy and pasted) into your "Terminal" program.
</p><p>When using Debian or Ubuntu:
</p>
<pre>   sudo aptitude update;
   sudo aptitude install libpng12-dev zlibc zlib1g-dev libtiff-dev 
   libungif4-dev libjpeg-dev libxml2-dev libuninameslist-dev 
   xorg-dev subversion cvs gettext git libpango1.0-dev 
   libcairo2-dev;
</pre>
<p>and enter your password when prompted.
</p><p>When using Fedora or Red Hat:
</p>
<pre>   su;
   yum update;
   yum install libpng-devel zlib-devel libtiff-devel giflib-devel 
   libjpeg-devel libxml2-devel libuninameslist-devel cairo-devel 
   python-devel cvs git subversion mercurial pango-devel;
   yum groupinstall x-software-development development-tools;
   exit;
</pre>
<p>and enter the root password when prompted.
</p>
<a id="Download_FontForge_source_code" name="Download_FontForge_source_code"></a><h4> <span class="mw-headline"> Download FontForge source code </span></h4>
<p>First, use the 'change directory' command "cd" to ensure you are in your 'home directory' ("~"). Then make a "source code" folder with the 'make directory' command "mkdir" to keep things tidy. Then change to that directory.
</p>
<pre>   cd ~;
   mkdir src;
   cd src;
</pre>
<p>FontForge source code is kept in a "CVS" version control system operated by the SourceForge website. First, login to the SourceForge CVS server; hit the return key to enter a blank password when asked for one. Second, download the FontForge sourcecode:
</p>
<pre>   cvs -d:pserver:anonymous@fontforge.cvs.sourceforge.net:/cvsroot/fontforge login;
   cvs -d:pserver:anonymous@fontforge.cvs.sourceforge.net:/cvsroot/fontforge co fontforge;
</pre>
<a id="Download_other_sourcecode" name="Download_other_sourcecode"></a><h4> <span class="mw-headline"> Download other sourcecode </span></h4>
<p>Using the CVS and the Subversion ("SVN") version control programs, download the other source code to enable all of FontForge's features: Freetype2 is a text rendering system used to draw fonts on screen, and libspiro is the Spiro drawing program that is integrated into FontForge.
</p>
<pre>   git clone git://git.sv.gnu.org/freetype/freetype2.git;
   git clone git://git.sv.gnu.org/freetype/freetype2-demos.git;
   svn co <a title="http://libspiro.svn.sourceforge.net/svnroot/libspiro/" class="external free" href="http://libspiro.svn.sourceforge.net/svnroot/libspiro/">http://libspiro.svn.sourceforge.net/svnroot/libspiro/</a>;
</pre>
<p>If you live in a country without software-idea patents (such as a European country, but not the USA) you can make a small change to the freetype source code to enable FontForge's hinting features. If you live in a country with software idea patents, to legally use these features you should obtain a TrueType hinting patent license from Apple. Open this file:
</p>
<pre>   freetype2/include/freetype/config/ftoption.h
</pre>
<p>and change
</p>
<pre>   /* #define TT_CONFIG_OPTION_BYTECODE_INTERPRETER */
</pre>
<p>to
</p>
<pre>   #define TT_CONFIG_OPTION_BYTECODE_INTERPRETER
</pre>
<p>then save and close it.
</p>
<a id="Compile.2C_install_and_run_FontForge" name="Compile.2C_install_and_run_FontForge"></a><h4> <span class="mw-headline"> Compile, install and run FontForge </span></h4>
<p>These 3 commands change to the libspiro directory, configure and compile the program:
</p>
<pre>   cd ~/src/libspiro;
   ./configure;
   make;
</pre>
<p>To install programs you compile, you need root access. With some distributions, like Ubuntu, root access is available with the "sudo" command and your own password:
</p>
<pre>   sudo make install;
</pre>
<p>On other distributions, such as Fedora, that command may not work. If not, root access is available with the "su" command and the root password:
</p>
<pre>   su; make install; exit
</pre>
<p>Now configure, compile and install FontForge:
</p>
<pre>   cd ~/src/fontforge/;
   ./configure --enable-pyextension --enable-type3 --enable-pasteafter 
   --enable-tilepath --enable-double --enable-device-tables 
   --with-capslock-for-alt --with-freetype-bytecode 
   --with-freetype-src=../freetype2 --with-x --with-pango;
   make;  
   sudo make install;
</pre>
<p>or
</p>
<pre>   su; make install; exit
</pre>
<p>(on Fedora, su to become root and then run make install)
</p><p>Finally, run FontForge:
</p>
<pre>   /usr/local/bin/fontforge;
</pre>

<h4> Updating your source code </h4>
<p>You don't have to do all this each time you want to update. Just run the following commands:
</p>
<pre>   cd ~/src/libspiro; make clean; svn up; ./configure; make; sudo make install;
   cd ~/src/freetype2; git pull;
   cd ~/src/fontforge; sudo make clean; cvs up -Cd;
   ./configure --enable-pyextension --enable-type3 --enable-pasteafter 
   --enable-tilepath --with-capslock-for-alt --with-freetype-bytecode 
   --with-freetype-src=../freetype2 --with-x;
   make; sudo make install;
</pre>
<p><br>
</p>
<hr>
<p>We also publish other information about <a title="FontForge" href="/wiki/FontForge">FontForge</a>, including <a title="How to setup FontForge" href="/wiki/How_to_setup_FontForge">How to setup FontForge</a>.
</p>