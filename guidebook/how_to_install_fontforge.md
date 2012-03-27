<h1>How To Install FontForge</h1>

<p>This page is step by step guide to installing <a title="FontForge" href="/wiki/FontForge">FontForge</a> for beginners.
</p><p>The first part covers installing FontForge's "official" releases.
</p><p>The second part of this page explains how some FontForge users install the "source code" version of FontForge. Many people do this so they can use the very latest features, and have the very latest bug fixes. This version is updated almost daily. If you want to report a problem of FontForge, we recommend that you try reproducing your problem with the source code version - you may find your problem has already been fixed! We explain how to install FontForge from source code both for the first time, and how to update it too.
</p>
<h4>Contents</h4>
<ul>
<li class="toclevel-1"><a href="#Official_Releases"><span class="tocnumber">1</span> <span class="toctext">Official Releases</span></a>
<ul>
<li class="toclevel-2"><a href="#Mac_OS_X"><span class="tocnumber">1.1</span> <span class="toctext">Mac OS X</span></a></li>
</ul>
</li>
<li class="toclevel-1"><a href="#Source_Code"><span class="tocnumber">2</span> <span class="toctext">Source Code</span></a>
<ul>
<li class="toclevel-2"><a href="#GNU.2FLinux"><span class="tocnumber">2.1</span> <span class="toctext">GNU/Linux</span></a>
<ul>
<li class="toclevel-3"><a href="#Install_the_required_programs"><span class="tocnumber">2.1.1</span> <span class="toctext">Install the required programs</span></a></li>
<li class="toclevel-3"><a href="#Download_FontForge_source_code"><span class="tocnumber">2.1.2</span> <span class="toctext">Download FontForge source code</span></a></li>
<li class="toclevel-3"><a href="#Download_other_sourcecode"><span class="tocnumber">2.1.3</span> <span class="toctext">Download other sourcecode</span></a></li>
<li class="toclevel-3"><a href="#Compile.2C_install_and_run_FontForge"><span class="tocnumber">2.1.4</span> <span class="toctext">Compile, install and run FontForge</span></a></li>
</ul>
</li>
<li class="toclevel-2"><a href="#Mac_OS_X_2"><span class="tocnumber">2.2</span> <span class="toctext">Mac OS X</span></a></li>
<li class="toclevel-2"><a href="#Updating_your_source_code"><span class="tocnumber">2.3</span> <span class="toctext">Updating your source code</span></a></li>
</ul>
</li>
</ul>
</td></tr></tbody></table><script type="text/javascript"> if (window.showTocToggle) { var tocShowText = "show"; var tocHideText = "hide"; showTocToggle(); } </script>
<h4> Official Releases </h4>
<p><b>Please edit this page and explain how to install FontForge step by step for Ubuntu, Fedora, Mac OS X and Windows!</b>
</p><p><a title="https://sourceforge.net/project/showfiles.php?group_id=103338&package_id=111040" class="external text" href="https://sourceforge.net/project/showfiles.php?group_id=103338&package_id=111040">On the SourceForge Download page</a> you will see a list of 7 versions of FontForge. These are for the various kinds of computers people use today, and their names are packed with technical details. This means they can seem a little cryptic, so here is our guide to them:
</p>
<ul><li> <b>GNU/Linux on 32 bit PCs</b>: fontforge-YYYYMMDD.i386.rpm
</li><li> <b>GNU/Linux on 64 bit PCs</b>: fontforge-YYYYMMDD.x86_64.rpm
</li></ul>
<ul><li> <b>Windows with Cygwin installed</b>: fontforge_cygwin-YYYYMMDD.tar.bz2
</li></ul>
<ul><li> <b>Intel Macs with Leopard</b>: FontForge_intelmacX.5_x86-py25-YYYYMMDD.pkg.zip
</li><li> <b>G3, G4 or G5 Macs with Leopard</b>: FontForge_macX.5_ppc-py25-YYYYMMDD.pkg.zip
</li></ul>
<ul><li> <b>Intel Macs with Tiger</b>: FontForge_intelmacX.4_x86-py23-YYYYMMDD.pkg.zip
</li><li> <b>G3, G4 or G5 Macs with Tiger</b>: FontForge_macX.4_py2.3-YYYYMMDD.pkg.zip
</li></ul>
<p>These examples include "YYYYMMDD" that will appear as numbers for the year, month and date of publication (eg, 20081103).
</p><p>The FontForge manual contains instructions for installing these packages on <a title="http://fontforge.sourceforge.net/nix-install.html" class="external text" href="http://fontforge.sourceforge.net/nix-install.html">GNU/Linux</a>, <a title="http://fontforge.sourceforge.net/mac-install.html" class="external text" href="http://fontforge.sourceforge.net/mac-install.html">Mac OS X</a> and <a title="http://fontforge.sourceforge.net/ms-install.html" class="external text" href="http://fontforge.sourceforge.net/ms-install.html">Windows</a>. There is also an <a title="http://www.geocities.jp/meir000/fontforge/" class="external text" href="http://www.geocities.jp/meir000/fontforge/">Unofficial Windows Version</a>.
</p>
<h4> Mac OS X </h4>
<p><b>Please edit this line with exact details on how to do each step</b>
</p><p>To solve copy-paste problems with FontForge and also Inkscape, change the X11 preferences' "Pasteboard" settings to that "Enable syncing" is disabled.
</p><p>The best way to experience free software like FontForge is to run GNU/Linux on your Mac. When you use FontForge on Mac OS X, you make it much easier to move to GNU/Linux in the future.
</p><p>0. Go to the Apple menu and run "Software Update" and make sure all the "Mac OS X Update" items are installed. 
</p><p>1. Insert the Mac OS X installation DVD and install X11: Browse the disc and scroll down to "Optional Installs" and open it. Keep clicking Continue until you get to the pane "Custom Install on Macintosh HD." Press the arrow beside "Applications so you get a list of them. Select X11 and keep pressing Continue.
</p><p>2. Download and install the 'libraries' from 
<a title="http://downloads.sourceforge.net/sourceforge/fontforge/FFLibs-intelmac-20081207.pkg.zip" class="external free" href="http://downloads.sourceforge.net/sourceforge/fontforge/FFLibs-intelmac-20081207.pkg.zip">http://downloads.sourceforge.net/sourceforge/fontforge/FFLibs-intelmac-20081207.pkg.zip</a>
</p><p>3. Download and install FontForge from <a title="http://downloads.sourceforge.net/fontforge/FontForge_intelmacX.5_x86-py25-20090224.pkg.zip" class="external free" href="http://downloads.sourceforge.net/fontforge/FontForge_intelmacX.5_x86-py25-20090224.pkg.zip">http://downloads.sourceforge.net/fontforge/FontForge_intelmacX.5_x86-py25-20090224.pkg.zip</a>
</p><p>4. Create a text file  in your home directory with this name (not the period at the start)
</p>
<pre>   .fonts.conf
</pre>
<p>And make it contain the following:
</p>
<pre>   <?xml version="1.0"?>
   <!DOCTYPE fontconfig SYSTEM "fonts.dtd">
   <fontconfig>
           <dir>/System/Library/Fonts</dir>
           <dir>/Library/Fonts</dir>
           <dir>~/Library/Fonts</dir>
   </fontconfig>
</pre>
<p>5. Go to the Finder and find the FontForge application in /Applications, and drag it to your Dock.
</p><p>6. Run run FontForge from the Dock.
</p>
<h4> Source Code </h4>
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
<h4>  Mac OS X</h4>
<p>The procedure for installing FontForge from source code on Mac OS X is the same as for GNU/Linux, above, except that installing the depencies is different. If you install FontForge from source on Mac OS X successfully from scratch, please write up your steps here. 
</p><p>The official FontForge website has a page about <a title="http://fontforge.sourceforge.net/MacOSX.html" class="external text" href="http://fontforge.sourceforge.net/MacOSX.html">installing FontForge on Mac OS X</a> too.
</p>
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