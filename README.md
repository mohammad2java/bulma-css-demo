setup-include following into header
--------------------------------------
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.5/css/bulma.min.css">

layout management
------------------
    
    The .container class can be used in any context, but mostly as a direct child of either:
        .navbar
        .hero
        .section
        .footer
    
    
layout header section  (header = logo+left-menu+right-menu)
------------------------
    1- create nav tag with navbar class n(this is complete header)
    2- for logo use navbar-brand with div tag and use navbar-item for logo and link
    3- for menu (left+right) use navbar-menu 
    4- for left menu use  navbar-start
    5- for right menu use navbar-end
    
    example:
    
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
        </a>

        <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item">
            Home
          </a>

          <a class="navbar-item">
            Documentation
          </a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">
              More
            </a>

            <div class="navbar-dropdown">
              <a class="navbar-item">
                About
              </a>
              <a class="navbar-item">
                Jobs
              </a>
              <a class="navbar-item">
                Contact
              </a>
              <hr class="navbar-divider">
              <a class="navbar-item">
                Report an issue
              </a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <a class="button is-primary">
                <strong>Sign up</strong>
              </a>
              <a class="button is-light">
                Log in
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>
    
-->> in bootstrap we use row and col-md-5 concept
--------------------------------------------------    
    in bulma we use columns  instead of row and column for each col-md-* section of columns
    bydefault all column will divide screen in equal partition. if you want to specifies the width of cloumn you can specify in following ways
    If you want to change the size of a single column, you can use one of the following classes:
    is-three-quarters
    is-two-thirds
    is-half
    is-one-third
    is-one-quarter
    is-full
    is-four-fifths
    is-three-fifths
    is-two-fifths
    is-one-fifth
    
    12 columns system #
    -----------------
        As the grid can be divided into 12 columns, there are size classes for each division:
        is-1
        is-2
        is-3
        is-4
        is-5
        is-6
        is-7
        is-8
        is-9
        is-10
        is-11
        is-12
        
        Offset #
        -------
        While you can use empty columns (like <div class="column"></div>) to create horizontal space around .column elements, you can also use offset modifiers like .is-offset-x:
        
        
        
        
    
responsiveness management
-------------------------
    add is-mobile to columns and make page mobile friendly
    <div class="columns is-mobile">
    </div>




color management
----------------
    1) background color
    --------------------
    has-background-X    example has-background-red,has-background-info,has-background-success
    
    for form element backgroud can do in following ways also
    ----------------------------------------------------------
     is-x   example: is-info,is-success  etc..

    2) for fond color
    -----------------
    has-text-X     example: has-text-red,has-text-info,has-text-success
    
    
    