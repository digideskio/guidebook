<h1>Collaborative Design Workflows</h1>

<p>You can call a typeface a work of art, a design, or a computer program: all these denominers make sense. What these three things have in common is that they are systems of signs, wherein every part is dependent on every other part.
</p><p>This makes the possibillity of collaboration inevident; to have such a system to be contained within one creative mind seems to be the most logical approach, as it assures a coherent approach to the different levels of structure within such a project.
</p><p>However, many art and design projects just don’t fit into one mind only. Even though a movie can be said to express the vision of its director, it is also the result of the collaboration between the director and a thousand other people, whose talents have all in one way or the other contributed to the end result.
</p><p>Similarly, many visual artists now work as producers, assembling teams and acquiring skills as required by the subject matter at hand.
</p><p>And with computer programs, of course, collaboration has been evident ever since they were written, as they were conceived in the sphere of Science.
</p><p>The highly interesting question is, IEHO, if we can map the collaboration mechanisms as devised within the free software movement, to the production of cultural artefacts, in this case typefaces.
</p>
<h4> Contents </h4> 
<p>
<ul>
<li class="toclevel-2"><a href="#Versioning_.28revision_control.29"><span class="tocnumber">1</span> <span class="toctext">Versioning (revision control)</span></a>
<ul>
<li class="toclevel-2"><a href="#Centralised_and_distributed_versioning"><span class="tocnumber">1.1</span> <span class="toctext">Centralised and distributed versioning</span></a></li>
<li class="toclevel-2"><a href="#Versioning_Systems"><span class="tocnumber">1.2</span> <span class="toctext">Versioning Systems</span></a></li>
<li class="toclevel-2"><a href="#Workflows_and_tools"><span class="tocnumber">1.3</span> <span class="toctext">Workflows and tools</span></a></li>
</ul>
</li>
</ul>
</td></tr></tbody></table><script type="text/javascript"> if (window.showTocToggle) { var tocShowText = "show"; var tocHideText = "hide"; showTocToggle(); } </script>
<a id="Versioning_.28revision_control.29" name="Versioning_.28revision_control.29"></a><h4> Versioning (revision control) </h4>
<blockquote>
Revision control (also known as version control, source control or (source) code management (SCM)) is the management of changes to documents, programs, and other information stored as computer files. It is most commonly used in software development, where a team of people may be changing the same files.
</blockquote>
<h4> Centralised and distributed versioning </h4>
<blockquote>
Distributed revision control (DRCS) takes a peer-to-peer approach, as opposed to the client-server approach of centralized systems. Rather than a single, central repository on which clients synchronize, each peer’s working copy of the codebase is a bona-fide repository. Synchronization is conducted by exchanging patches (change-sets) from peer to peer.
</blockquote>
<h4> Versioning Systems </h4>
<ul><li> Centralised
<ul><li> CVS was the first widely used free tool. SVN is the one that is currently ubiquitous.
</li></ul>
</li><li> Distributed
<ul><li> Darcs, Mercurial, Git and Bazaar are the main software packages used right now. All are free.
</li></ul>
</li><li> Hosted
<ul><li> <a title="http://sourceforge.net" class="external text" href="http://sourceforge.net">Sourceforge</a> (SVN)
</li><li> <a title="https://launchpad.net/" class="external text" href="https://launchpad.net/">Launchpad</a> (Bazaar)
</li><li> <a title="http://freehg.org/" class="external text" href="http://freehg.org/">FreeHG</a> (Mercurial)
</li><li> <a title="http://github.com/" class="external text" href="http://github.com/">GitHub</a> (Git)
</li></ul>
</li></ul>
<p>You will probably not want to go through the hassle of configuring a server with version control software; it most cases it is probably the most practical to choose a hosted service.
</p><p>The other choice is between distributed and centralised, IEHO distributed versioning is more suited to dealing with cultural artefacts than centralised versioning; it allows and even promotes variation between different copies of the same repository. This might be unhandy sometimes with computer software—with cultural artefacts it is the way go to achieve the pluriformity and personality we associate with culture in the first place.
</p><p>Simon Pascal Klein shows how to use GitHub to fork the OpenBaskerville project, which is as trivial as geek gets, @ <a title="http://klepas.org/openbaskerville/#using-git" class="external free" href="http://klepas.org/openbaskerville/#using-git">http://klepas.org/openbaskerville/#using-git</a>
</p><p>In a rather spectacular turn of events (at least in my mind) GitHub recently implemented UFO support, including visual diffs: <a title="http://github.com/rbmntjs/open-baskerville/commit/c5b3322fb49baa3104363ca98546c684d940c0ef" class="external free" href="http://github.com/rbmntjs/open-baskerville/commit/c5b3322fb49baa3104363ca98546c684d940c0ef">http://github.com/rbmntjs/open-baskerville/commit/c5b3322fb49baa3104363ca98546c684d940c0ef</a>
</p><p>And visualisations of UFO typefaces:
<a title="http://github.com/rbmntjs/open-baskerville/tree/bc03fca9968df8683b3df2ae9afb0185c4acf433/OpenBaskerville.ufo" class="external free" href="http://github.com/rbmntjs/open-baskerville/tree/bc03fca9968df8683b3df2ae9afb0185c4acf433/OpenBaskerville.ufo">http://github.com/rbmntjs/open-baskerville/tree/bc03fca9968df8683b3df2ae9afb0185c4acf433/OpenBaskerville.ufo</a>
</p><p>
</p>
<h4> Workflows and tools </h4>
<p>The <a title="http://freehg.org/u/taejo/ffhg/" class="external text" href="http://freehg.org/u/taejo/ffhg/">ff-hg python plugin for FontForge</a> is a simple interface to the Mercurial version control system. To install it, make sure you have Mercurial installed using your operating system's usual way. Then open the Terminal and run the following command:
</p>
<pre>   mkdir ~/.FontForge/python; cd ~/.FontForge/python; 
   curl -O <a title="http://freehg.org/u/taejo/ffhg/raw-file/tip/ffhg.py" class="external free" href="http://freehg.org/u/taejo/ffhg/raw-file/tip/ffhg.py">http://freehg.org/u/taejo/ffhg/raw-file/tip/ffhg.py</a>
</pre>
<p><a title="http://freehg.org/u/taejo/ffhg/raw-file/tip/docs/walkthru.html" class="external text" href="http://freehg.org/u/taejo/ffhg/raw-file/tip/docs/walkthru.html">The ff-hg walkthrough</a> has more details.
</p><p>Debian has an <a title="http://svn.debian.org/wsvn/pkg-fonts/foo-open-font-sources/" class="external text" href="http://svn.debian.org/wsvn/pkg-fonts/foo-open-font-sources/">Overview of a complete set of files and sources (with links) for VCS (version control system) development and release branch of an open font.</a>
</p><p>The lazyhandwriterfont project has published some <a title="http://bazaar.launchpad.net/~gryc-ueusp/lazyhandwriterfont/main/files/head%3A/scripts/" class="external text" href="http://bazaar.launchpad.net/~gryc-ueusp/lazyhandwriterfont/main/files/head%3A/scripts/">scripts for importing SVG files into FontForge</a>
</p><p><a title="http://sourceforge.net/projects/fonttools/" class="external text" href="http://sourceforge.net/projects/fonttools/">TTX</a> is a tool to convert OpenType and TrueType fonts to and from XML. FontTools is a library for manipulating fonts, written in Python. It supports TrueType, OpenType, AFM and to an extent Type 1 and some Mac-specific formats.
</p><p><a title="http://robofab.org/" class="external text" href="http://robofab.org/">RoboFab</a> is a Python library with objects that deal with data usually associated with fonts and type design. It writes and reads UFOs. There is an <a title="http://www.lowest-common-denominator.com/2007/03/svn_helper_script_for_robobab.php" class="external text" href="http://www.lowest-common-denominator.com/2007/03/svn_helper_script_for_robobab.php">SVN helper script for Robofab</a> by Brook Elgie
</p><p><a title="http://meld.sourceforge.net" class="external text" href="http://meld.sourceforge.net">Meld</a> is a visual diff and merge tool. 
</p><p>How do you programmaticaly go from a UFO or SFD to OTF files? FontForge's python makes this simple, and Dave Crossland published a simple <a title="http://article.gmane.org/gmane.comp.freedesktop.fonts/1741" class="external text" href="http://article.gmane.org/gmane.comp.freedesktop.fonts/1741">conversion script</a> on the OFLB mailing linst.
</p>