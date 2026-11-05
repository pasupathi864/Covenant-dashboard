Royalty Signals prototypes - standalone build

Files
  index.html     opens Option 1
  option-1.html  Deals and revenue tabs (popup for operator details)
  option-2.html  Split view (deal list + operator panel)

Each file is self-contained: HTML, CSS, sample data and logic are inline.
The only external request is the Inter font from Google Fonts; without it the
pages fall back to the system font.

Hosting
  Copy the folder to any static host (internal web server, IIS, nginx,
  SharePoint/Teams site that serves .html, S3/Azure Blob static site, GitHub
  Pages on an internal org). No build step or server code is needed.
  Opening option-1.html directly from disk also works.

Editing
  Sample data (deals, operators, flags, values) is in the <script> block near
  the end of each file: DEALS, DOS, VALUES, SIGNED_AGO and REVF.
  The page markup is in the <script type="text/x-template" id="tpl"> block and
  uses {{name}} bindings, <sc-for> loops and <sc-if> conditions.
  "Open in Pixie" buttons link to #chat; replace href="#chat" with the real
  Pixie chat URL when it exists.
