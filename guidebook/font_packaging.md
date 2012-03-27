<h1>Font Packaging</h1>

<p>This page deals with all distribution-related topics.
</p>
<h4> Font archive naming </h4>
<p>If the font has a suitable license and gets accepted to Debian/Ubuntu/Fedora, for example, it will acquire a name of the form <i>ttf-foundryname-fontfamilyname"</i>
</p><p>The actually package could be <i>ttf-oflb-myfont.1.0.zip</i> (or <i>ttf-oflb-myfont.1.0.7z</i>, or <i>ttf-oflb-myfont.1.0.tar.gz</i>)
</p><p>The package should contains as much of the extended font source as possible.
</p><p>Regarding the version numbers please follow the binary version field in the ttf itself.
</p><p><br>
</p>
<h4> Font Headers </h4>
<p>TrueType and Postscript fonts possess headers which can bear meta information. Amongst others, there are standard fields for
</p>
<ul><li> creator
</li><li> creation date
</li><li> copyright
</li><li> trademark
</li><li> notice/description
</li><li> designer
</li><li> designer url
</li><li> vendor
</li><li> url
</li><li> license
</li><li> license url
</li><li> version
</li><li> truetype version record
</li><li> truetype vendor code
</li><li> font creation date
</li></ul>
<p>and several more.
</p><p><br>
See <a title="Font metadata" href="/wiki/Font_metadata">font_metadata</a> for details. 
</p><p>Packaging is best left to distro teams like the <a title="http://fedoraproject.org/wiki/SIGs/Fonts" class="external text" href="http://fedoraproject.org/wiki/SIGs/Fonts">Fedora font SIG</a> and the <a title="http://pkg-fonts.alioth.debian.org/" class="external text" href="http://pkg-fonts.alioth.debian.org/">Debian font task force</a> but encouraging designers uploading to OFL to follow best practises will help everyone.
</p>
