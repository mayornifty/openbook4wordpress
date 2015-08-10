<h1>OpenBook Template Elements</h1>

<p>Using OpenBook is as simple as placing a shortcode in a WordPress post, page or widget, e.g., <code>[openbook booknumber="1234"]</code> where <code>"1234"</code> is an ISBN or Open Library key, or using the OpenBook button the WordPress Visual Editor. Nothing more is required. OpenBook will use the default templates to display a book cover, title, author, publisher, and links. This help file is intended for people who want to have more control over the content, ordering, and styling of the display.</p>

<h2>OpenBook Templates</h2>

<p>The templates are managed in the Settings|OpenBook panel of WordPress dashboard. There are three templates. The first template is used by default. You can use one of the other templates by specifying the template number inline with the shortcode, e.g., <code>[openbook booknumber="1234" templatenumber="2"]</code>, or by selecting the template number from the list after clicking the OpenBook button in the Visual Editor .</p>

<h2>Display Elements</h2>

<p>Templates determine what OpenBook displays. Templates can contain any text or HTML you want to display. As you see in the default templates, they also contain display elements, items in square brackets. When OpenBook finds one of the display elements, it replaces it with a predefined block of text or HTML. E.g., the <code>[OB_COVER_MEDIUM]</code> display element shows an Open Library book cover image of medium size with a link to Open Library. The elements make template assembly easy.</p>

<p>An item is only displayed if it is available in the Open Library book record. If it is missing, you can add it using the Open Library web page for the book.</p>

<h3>Open Library Display Elements</h3>

<p>There are two types of display elements: Open Library and OpenBook. The Open Library elements are the root elements used by the OpenBook elements. The OpenBook elements are richer in features, but the Open Library elements give you more control.</p>


<p>
<table>
<tr><td>Display Element</td><td>Description</td></tr>
<tr><td><code>[OL_URL]</code></td><td>Url of Open Library web page</td></tr>
<tr><td><code>[OL_COVER_SMALL]</code></td><td>Url of small-sized cover image</td></tr>
<tr><td><code>[OL_COVER_MEDIUM]</code></td><td>Url of medium-sized cover image</td></tr>
<tr><td><code>[OL_COVER_LARGE]</code></td><td>Url of large-sized cover image</td></tr>
<tr><td><code>[OL_TITLE]</code></td><td>Title</td></tr>
<tr><td><code>[OL_SUBTITLE]</code></td><td>Subtitle</td></tr>
<tr><td><code>[OL_AUTHORLIST]</code></td><td>List of authors</td></tr>
<tr><td><code>[OL_AUTHORURLLIST]</code></td><td>List of links to Open Library author pages</td></tr>
<tr><td><code>[OL_AUTHORFIRST]</code></td><td>First author</td></tr>
<tr><td><code>[OL_AUTHORURLFIRST]</code></td><td>First author URL</td></tr>
<tr><td><code>[OL_BYSTATEMENT]</code></td><td>By statement</td></tr>
<tr><td><code>[OL_PUBLISHERLIST]</code></td><td>List of publishers</td></tr>
<tr><td><code>[OL_PUBLISHERFIRST]</code></td><td>First publisher</td></tr>
<tr><td><code>[OL_PUBLISHPLACELIST]</code></td><td>List of publish places</td></tr>
<tr><td><code>[OL_PUBLISHPLACEFIRST]</code></td><td>First publish place</td></tr>
<tr><td><code>[OL_PUBLISHDATE]</code></td><td>Publish date</td></tr>
<tr><td><code>[OL_PAGINATION]</code></td><td>Pagination</td></tr>
<tr><td><code>[OL_PAGES]</code></td><td>Pages</td></tr>
<tr><td><code>[OL_WEIGHT]</code></td><td>Weight</td></tr>

<tr><td><code>[OL_ID_AMAZON]</code></td><td>Amazon ID</td></tr>
<tr><td><code>[OL_ID_GOODREADS]</code></td><td>Goodreads ID</td></tr>
<tr><td><code>[OL_ID_GOOGLE]</code></td><td>Google Books ID</td></tr>
<tr><td><code>[OL_ID_ISBN10]</code></td><td>ISBN 10 digit</td></tr>
<tr><td><code>[OL_ID_ISBN13]</code></td><td>ISBN 13 digit</td></tr>
<tr><td><code>[OL_ID_LCCN]</code></td><td>Library of Congress Cataloging Number</td></tr>
<tr><td><code>[OL_ID_LIBRARYTHING]</code></td><td>LibraryThing ID</td></tr>
<tr><td><code>[OL_ID_OCLCWORLDCAT]</code></td><td>WorldCat ID</td></tr>
<tr><td><code>[OL_ID_PROJECTGUTENBERG]</code></td><td>Project Gutenberg ID</td></tr>
<tr><td><code>[OL_ID_OPENLIBRARY]</code></td><td>Open Library ID</td></tr>
<tr><td><code>[OL_ISBN]</code></td><td>13 digit ISBN if available, else 10 digit ISBN, else blank</td></tr>
<tr><td><code>[OL_SUBJECTLIST]</code></td><td>List of subjects</td></tr>
<tr><td><code>[OL_PREVIEW_URL]</code></td><td>Indicates if an ebook version is available</td></tr>
<tr><td><code>[OL_LINKTITLES]</code></td><td>A list of link titles, goes with the link URLs</td></tr>
<tr><td><code>[OL_LINKURLS]</code></td><td>A list of links</td></tr>
<tr><td><code>[OL_LINKTITLEFIRST]</code></td><td>First link title</td></tr>
<tr><td><code>[OL_LINKURLFIRST]</code></td><td>First link URL</td></tr>
<tr><td><code>[OL_EXCERPT_COMMENT_FIRST]</code></td><td>First excerpt comment</td></tr>
<tr><td><code>[OL_EXCERPT_TEXT_FIRST]</code></td><td>First excerpt</td></tr>
</table>

<h3>OpenBook Display Elements</h3>

<p>OpenBook display elements use Open Library display elements and other data to construct more complex HTML display elements.</p>

<p>
<table>
<tr><td>Display Element</td><td>Description</td></tr>
<tr valign='top'><td><code>[OB_COVER_SMALL]</code></td><td>Small cover with descriptive hover text where available, and link to Open Library</td></tr>
<tr valign='top'><td><code>[OB_COVER_MEDIUM]</code></td><td>Medium cover with descriptive hover text where available, and link to Open Library</td></tr>
<tr valign='top'><td><code>[OB_COVER_LARGE]</code></td><td>Large cover with descriptive hover text where available, and link to Open Library</td></tr>
<tr valign='top'><td><code>[OB_TITLE]</code></td><td>Title with link to Open Library book record</td></tr>
<tr valign='top'><td><code>[OB_AUTHORS]</code></td><td>Author name with link to Open Library author record</td></tr>
<tr valign='top'><td><code>[OB_PUBLISHER]</code></td><td>Publisher with link to publisher website if provided as inline parameter</td></tr>
<tr valign='top'><td><code>[OB_PUBLISHYEAR]</code></td><td>Year the work was published</td></tr>
<tr valign='top'><td><code>[OB_READONLINE]</code></td><td>Link to scanned work online, if available</td></tr>
<tr valign='top'><td><code>[OB_LINK_FINDINLIBRARY]</code></td><td>Link to a particular library's records if an OpenURL resolver is configured in Settings</td></tr>
<tr valign='top'><td><code>[OB_IMAGE_FINDINLIBRARY]</code></td><td>Image link to a particular library's records, if an image source and OpenURL resolver is configured in Settings</td></tr>
<tr valign='top'><td><code>[OB_COINS]</code></td><td>Invisible bibliographic for detection by other applications like Zotero</td></tr>
<tr valign='top'><td><code>[OB_LINKS]</code></td><td>List of formatted links</td></tr>
<tr valign='top'><td><code>[OB_LINK_AMAZON]</code></td><td>Link to Amazon record</td></tr>
<tr valign='top'><td><code>[OB_LINK_GOODREADS]</code></td><td>Link to Goodreads record</td></tr>
<tr valign='top'><td><code>[OB_LINK_GOOGLEBOOKS]</code></td><td>Link to Google Books record</td></tr>
<tr valign='top'><td><code>[OB_LINK_LIBRARYCONGRESS]</code></td><td>Link to Library of Congress record</td></tr>
<tr valign='top'><td><code>[OB_LINK_LIBRARYTHING]</code></td><td>Link to LibraryThing record</td></tr>
<tr valign='top'><td><code>[OB_LINK_WORLDCAT]</code></td><td>Link to WorldCat record</td></tr>
<tr valign='top'><td><code>[OB_LINK_PROJECTGUTENBERG]</code></td><td>Link to Project Gutenberg record</td></tr>
<tr valign='top'><td><code>[OB_LINK_BOOKFINDER]</code></td><td>Link to BookFinder record</td></tr>
<tr valign='top'><td><code>[OB_DOT]</code></td><td>A 'bullet' style delimiter. If an element is missing, OpenBook prevents duplicate dots from appearing beside each other.</td></tr>

</table>