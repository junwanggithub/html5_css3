HTML5 Form
=========================


Form attributes
------------------

Required attribute
^^^^^^^^^^^^^^^^^^^
::

    <form>
    <ul>
      <li>
        <label for="url">My website is located at:</label>
        <input type="text" id="url" name="url" required>
      </li>
    </ul
    </form>

    //Define style
    input {
      background-position: 0% 50%;
      background-repeat: no-repeat;
      padding-left: 15px;
    }
    input:required {
      background-image: url('../images/required.png');
    }
    input:focus:invalid {
      background-image: url('../images/invalid.png');
    }
    input:focus:valid {
      background-image: url('../images/valid.png');
    }
    //for FF
    :invalid { box-shadow: none; }
    //for old browser
    input:required,
    input[required] {
      background-image: url('../images/required.png');
    }

.. raw:: html
    :file: ../_static/html5-form/required.html

The placeholder Attribute
^^^^^^^^^^^^^^^^^^^^^^^^^^^
::

    <input type="text" placeholder="please input your url" id="url" name="url">

.. raw:: html
    :file: ../_static/html5-form/required.html

The pattern Attribute
^^^^^^^^^^^^^^^^^^^^^^
::

    <input type="password" id="password" name="password" required
    title="(at least 6 characters, no spaces)" pattern="\S{6,}">

.. raw:: html
    :file: ../_static/html5-form/pattern.html

The disabled vs. readonly Attribute
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``disabled``   ``readonly``

.. raw:: html
    :file: ../_static/html5-form/disabled-readonly.html

Input type
------------------

Additional new form control in HTML5
--------------------------------------


Changes to exiting form controll
--------------------------------------

