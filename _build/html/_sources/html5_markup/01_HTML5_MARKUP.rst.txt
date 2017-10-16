HTML5 Basic Markup
=========================
A basic HTML5 template
----------------------
.. code:: html

    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="utf-8">
        <title>The HTML5 Herald</title>
        <meta name="description" content="The HTML5 Herald">
        <meta name="author" content="SitePoint">
        <link rel="stylesheet" href="css/styles.css">
        <!--[if lt IE 9]>
          <script src="js/html5shim.js"></script>
        <![endif]-->
      </head>
      <body>
        <script src="js/scripts.js"></script>
      </body>
    </html>

Small rules
------------
 *To balance between HTML5 cleaner syntax and consistency.*
    -  Use lowercase for all elements and attributes as you would in XHTML.
    -  Despite some elements not requiring closing tags, we recommend that all elements containing content be closed (as in <p>Text</p>).
    -  Although you can leave attribute values unquoted, it’s highly likely that you’ll have attributes that require quotes (for example, when declaring multiple classes separated by spaces, or when appending a query string value to a URL). As a result, we suggest that you always use quotes for the sake of consistency.
    -  Omit the trailing slash from void elements (such as meta or input).
    - Avoid providing redundant values for Boolean attributes (for instance, use <input type="checkbox" checked> rather than <input type="checkbox" checked="checked">).

Semantic page structure
------------------------
*The way a given HTML element describes the meaning of its content.*

Header element with a logo and title
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

    .. Attention:: A header element can be used to include introductory content or navigational aids that are specific to any single section of a page, or apply to the entire page, or both.

::

    Old:
    <div id="header">

    HTML5:
    <header></header>

Section element
^^^^^^^^^^^^^^^
    .. Attention:: A section element can be used as a container of generic thematic content. If it is more specific, use article, aside, or Nav; if hard to describe the content for special meaning, only description or style purpose, use <div>

::

    <section></section>

Article element
^^^^^^^^^^^^^^^
    .. Attention:: An article element is distributable or reusable for a complete, or self-contained composition

::

    <article></article>


Navigation element
^^^^^^^^^^^^^^^^^^^
.. Attention:: A navigation element is for wrapping an unordered list of links, except footer.

::

    <nav>
        <ul>
            <li><a href="#">World</a></li>
            <li><a href="#">National</a></li>
            <li><a href="#">Metro area</a></li>
            <li><a href="#">Sports</a></li>
            <li><a href="#">Arts &amp; Entertainment</a></li>
        </ul>
    </nav>

Aside element
^^^^^^^^^^^^^^^
    .. Attention:: An aside element is container of standalone to primary content,like Ad or friends links.

::

    <aside></aside>


Footer containing some author and copyright information
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. Attention:: An footer element is container of copyright information, lists of related links, author information, and similar information that you normally think of as coming at the end of a block of content.

::

    <footer></footer>

Main tag
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. Attention:: One document can only have one main tag.

::

    <main></main>

Wrapped up
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
::

    <body>
      <header>
        <nav></nav>
      </header>
      <main role="main">
            <div class="primary">
                <article></article>
            </div>
            <div class="secondary">
                <article></article>
            </div>
            <div class="tertiary">
              <aside>
                <article></article>
              </aside>
              <article>
              </article>
            </div>
      </main><!-- main -->
      <footer>
        <section id="authors">
          <section></section>
        </section>
        <section id="copyright">
        </section>
      </footer>
      <script src="js/scripts.js"></script>
    </body>

