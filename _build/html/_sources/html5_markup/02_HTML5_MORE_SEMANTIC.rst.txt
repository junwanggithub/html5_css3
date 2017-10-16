HTML5 More Semantic
=========================

More detailed HTML5 semantic elements for special meaning contents

More new elements
------------------

Figure element
^^^^^^^^^^^^^^^
::

    <article>
        <h1>Accessible Web Apps</h1>
        <p>Lorem ipsum dolor ... </p>
        <p>As you can see in <a href="#fig1">Figure 1</a>,
        <figure id="fig1">
            <figcaption>Screen Reader Support for WAI-ARIA</figcaption>
            <img src="figure1.png" alt="JAWS: Landmarks 1/1, Forms 4/5 ... ">
      </figure>
      <p>Lorem ipsum dolor ... </p>
    </article>

The mark Element
^^^^^^^^^^^^^^^^^
::

    <h1>Yes, You Can Use <mark>HTML5</mark> Today!</h1>

.. Attention:: em or strong; those elements add contextual importance; mark separates the targeted content based on a user’s current browsing or search activity.

The progress and meter elements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
::

    <progress value="22" max="100"></progress>
    <meter value="2" min="0" max="10">2 out of 10</meter><br>
    <meter value="0.6">60%</meter>

.. Attention:: Meter has known maximum value, for dynamic range should use progress bar

.. raw:: html
    :file: ../_static/html5_progress_meter_sample.html

The time element
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. Attention:: Time element is invaluable for SE to weight the search result


::

    Old:
    <p>We'll be getting together for our next developer conference on 12 October of this year.</p>
    HTML5:
    <p>We'll be getting together for our next developer conference on <time datetime="2015-10-12">12 October of this year</time>.</p>
    If datetime attr is missing, text of time tag should be a valid time format
    <!-- month -->
    <time>2015-11</time>
    <!-- date -->
    <time>2015-11-12</time>
    <!-- yearless date -->
    <time>11-12</time>
    <!-- time -->
    <time>14:54:39</time>
    <!-- floating date and time -->
    <time>2015-11-12T14:54:39</time>
    <!-- time-zone offset -->
    <time>-0800</time>
    <!-- global date and time -->
    <time>2015-11-12T06:54:39.929-0800</time>
    <!-- week -->
    <time>2015-W46</time>
    <!-- duration -->
    <time>4h 18m 3s</time>

Change to existing elements
---------------------------
``b``,  ``strong``, ``em``, ``small``, ``cite``
::

    <dl>
      <dt>Selector:</dt>
      <dd>The element(s) targeted.</dd>
      <dt>Property:</dd>
      <dd>The feature used to add styling to the targeted element, defined before a colon.</dd>
      <dt>Value:</dd>
      <dd>The value given to the specified property, declared after the colon.</dd>
    </dl>


Other new elements
---------------------------
The details Element
^^^^^^^^^^^^^^^^^^^^
::

    <details>
        <summary>Some Magazines of Note</summary>
      <ul>
        <li><cite>Bird Watcher's Digest</cite></li>
        <li><cite>Rower's Weekly</cite></li>
        <li><cite>Fishing Monthly</cite></li>
      </ul>
    </details>

.. raw:: html
    :file: ../_static/html5_detail_sample.html

Customized Ordered Lists
^^^^^^^^^^^^^^^^^^^^^^^^
::

    <ol>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>

    <ol start="50">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>

.. raw:: html
    :file: ../_static/html5_ol_sample.html

Scoped Styles
^^^^^^^^^^^^^
::

    <h1>Page Title</h1>
    <article>
      <style scoped>
        h1 {
          color: blue;
        }
      </style>
      <h1>Article Title</h1>
      <p>Article content.</p>
    </article>

The async Attribute for Scripts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Similar with defer, boolean attr, async used to control the loading order, used for independent js.

The picture element
^^^^^^^^^^^^^^^^^^^^

::

    <picture>
      <source media="(min-width: 650px)" srcset="img_pink_flowers.jpg">
      <source media="(min-width: 465px)" srcset="img_white_flower.jpg">
      <img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
    </picture>

Other notables
^^^^^^^^^^^^^^
``dialog``  ``download`` ``sandbox`` ``menu`` ``address``

The Future of Markup — Web Components?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



