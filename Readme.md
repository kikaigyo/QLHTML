#QLHTML 
Here is a very simple Quick Look generator for HTML files. It renders the HTML
code instead of the full HTML preview.

1) In Xcode, create a new project and chose Quick Look Plug-In template

2) Modify Info.plist file:

- change Plug-In bundle identifier to something meaningful
- change Document Types binding to public.html
- change "Needs to be run in main thread" to YES

3) Modify GenerateThumbnailForURL.c and GeneratePreviewForURL.c to render HTML
   content as plain text instead of HTML

4) Build and install in ~/Library/QuickLook or /Library/QuickLook

5) use "qlmanage -r" to make sure the Plug-In has been registered

6) Enjoy

via: <a href="https://github.com/jonasf73/QLHTML" title="jonasf73/QLHTML - GitHub" rel="nofollow" class="under_line">jonasf73/QLHTML - GitHub</a>
