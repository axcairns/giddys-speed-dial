<h1>
<sub>
<img src="https://raw.githubusercontent.com/axcairns/giddys-speed-dial/master/src/icons/icon32.png" height="32" width="32">
</sub>
Giddy's Speed Dial
</h1>

<h1>
<a href='https://addons.mozilla.org/firefox/addon/giddys-speed-dial/'><img alt='Get it for Firefox' src='https://github.com/axcairns/giddys-speed-dial/raw/master/assets/badges/ff-badge.png'/></a> <!--<a href='https://chrome.google.com/webstore/detail/giddys-speed-dial/imohnlganmafcmidafklgkgfgaagiohn'><img alt='Get it for Chrome' src='https://github.com/axcairns/giddys-speed-dial/raw/master/assets/badges/chrome-badge.png'/></a> <a href='https://microsoftedge.microsoft.com/addons/detail/kachajgmekhiajhbbfpfhbmonmpnpiee'><img src='https://github.com/axcairns/giddys-speed-dial/raw/master/assets/badges/microsoft-badge.png' alt='English badge' style='width: 166px; height: 60px;'/></a>-->
</h1>

A modern, cross-browser speed dial that respects your privacy, forked from https://github.com/conceptualspace/yet-another-speed-dial

As part of efforts to de-google myself I moved from Chrome to Firefox. On Chrome I had already set up bookmark synching to my home server and I found a chrome 'speed dial' extension which (albeit crudely) allowed me to navigate my bookmarks on the new tab page.

When I came to Firefox none of the speed dial extensions met my requirements, but one came close - <a href='https://addons.mozilla.org/firefox/addon/yet-another-speed-dial/'>Yet Another Speed Dial</a>. This extension was exquisitely beautiful but had one major missing feature - sub-folder support. I have A LOT of bookmarks and only being able to have one layer of folders was a deal breaker so I decided to fork.

Features -

- Automatically generates thumbnails and screenshots, or add your own.
- Uses the native bookmarks library so speed dials can be synced by the browser.
- Supports folders (including sub-folders!)
- Simple and fast UI
- No ads, trackers, or BS :)

Stuff I removed during the rebuild, either because I don't need those features or I broke them inadvertently. If these features float your boat I encourage you to try <a href='https://addons.mozilla.org/firefox/addon/yet-another-speed-dial/'>Yet Another Speed Dial</a>

 - drag and drop bookmarks (move to folder and reorder in folder)
 - add, edit and delete folders
 - add bookmark (can still edit and delete)
 - sort by age (my extension only sorts by name)

![alt tag](https://github.com/axcairns/giddys-speed-dial/raw/master/assets/screenshot.png)

## FAQ:

#### Can I use different images for the speed dials?
Yes! Just right-click the speed dial and select Edit.

#### One of my site thumbnails disappeared?
GSD loads thumbnails using the Open Graph standard. This keeps those thumbnails up to date automatically, but if a website removes the image it may no longer load in GSD. To fetch new images, simply right-click the dial and select "Refresh thumbnails".

#### Why does GSD require the "access your data for all websites" permission?
This is required for GSD to capture an image of the website for the thumbnail. **GSD accesses absolutely no other data for any reason whatsoever**. These two features (visual thumbnails and user privacy) were the primary motivation for creating GSD. Note, GSD still works if you deny this permission, just without capturing thumbnails. No information is collected of any kind. Source code is available to view <a href="https://github.com/axcairns/giddys-speed-dial">here</a>.

#### Why is GSD showing CPU usage in the Chrome task manager?
While the actual CPU usage is very low (confirm using your OS task manager), some cycles are used to elimate jankiness. GSD uses a high performance rendering engine (GSAP) to keep user interactions and animations smooth. The usage is 0 when GSD is not in focus.

#### Can I open speed dial links in Firefox Containers?
Yes, just use <kbd>Shift</kbd> + <kbd>Right-click</kbd> on the speed dial to access the default context menu.

#### Why isn't the address bar focused (active) by default on the new tab / home page?
This is a bug in Firefox: https://bugzilla.mozilla.org/show_bug.cgi?id=1411209
