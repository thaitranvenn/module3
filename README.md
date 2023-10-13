<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Assignment 4</title>
    <link rel="stylesheet" href="css/bootstrap.min.css" />
    <link rel="stylesheet" href="css/styles.css" />
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <link
      href="https://fonts.googleapis.com/css?family=Oxygen:400,300,700"
      rel="stylesheet"
      type="text/css"
    />
    <link
      href="https://fonts.googleapis.com/css?family=Lora"
      rel="stylesheet"
      type="text/css"
    />
    <style>
      /* Reset some default margin and padding */
      .navbar-brand h1 {
        font-size: 3em;
        margin-top: 0;
        margin-bottom: 0;
        text-align: left;
      }

      /* Basic styling for the outer boxes */
      .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 20px;
        padding: 20px;
      }

      /* Basic styling for the outer and inner boxes */
      .box {
        position: relative;
        padding: 20px;
        border: 5px solid black;
        background-color: rgb(141, 141, 141);
      }

      .inner-box {
        position: absolute;
        top: 0;
        right: 0;
        padding: 5px;
      }

      .inner-box-chicken {
        background-color: pink;
      }

      .inner-box-beef {
        background-color: rgb(208, 69, 69);
      }

      .inner-box-sushi {
        background-color: rgb(236, 232, 155);
      }

      /* Styling for the content */
      .content {
        margin-top: 30px;
        padding: 10px;
        text-align: center;
      }

      /* Styling for the titles */
      .title {
        font-size: 20px;
        font-weight: bold;
      }

      /* Media queries for responsive layout */

      /* Tablet */
      @media (min-width: 750px) and (max-width: 1199px) {
        .grid-container {
          grid-template-columns: repeat(2, 1fr);
        }

        .outer-box-sushi {
          grid-column: span 2;
        }
      }

      /* Mobile */
      @media (max-width: 750px) {
        .grid-container {
          grid-template-columns: repeat(1, 1fr);
        }
      }
    </style>
  </head>

  <body>
    <header>
      <nav id="header-nav" class="navbar navbar-default">
        <div class="container">
          <div class="navbar-header">
            <div class="navbar-brand">
              <h1>Food LLC</h1>
            </div>
            <button
              type="button"
              class="navbar-toggle collapsed"
              data-toggle="collapse"
              data-target="#collapsable-nav"
              aria-expanded="false"
            >
              <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
          </div>

          <div id="collapsable-nav" class="collapse navbar-collapse">
            <ul id="nav-list" class="nav navbar-nav navbar-right">
              <li>
                <a href="#">
                  <span></span
                  ><br class="hidden-xs" />
                  Chicken</a
                >
              </li>
              <li>
                <a href="#">
                  <span></span
                  ><br class="hidden-xs" />
                  Beef</a
                >
              </li>
              <li>
                <a href="#">
                  <span></span
                  ><br class="hidden-xs" />
                  Sushi</a
                >
              </li>
            </ul>
            <!-- #nav-list -->
          </div>
          <!-- .collapse .navbar-collapse -->
        </div>
        <!-- .container -->
      </nav>
      <!-- #header-nav -->
    </header>

    <div class="grid-container">
      <div class="box outer-box-chicken">
        <div class="inner-box inner-box-chicken">
          <div class="title">Chicken</div>
        </div>
        <div class="content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
          pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
          culpa qui officia deserunt mollit anim id est laborum.
        </div>
      </div>
      <div class="box outer-box-beef">
        <div class="inner-box inner-box-beef">
          <div class="title">Beef</div>
        </div>
        <div class="content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
          pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
          culpa qui officia deserunt mollit anim id est laborum.
        </div>
      </div>
      <div class="box outer-box-sushi">
        <div class="inner-box inner-box-sushi">
          <div class="title">Sushi</div>
        </div>
        <div class="content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
          pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
          culpa qui officia deserunt mollit anim id est laborum.
        </div>
      </div>
    </div>
    <!-- jQuery (Bootstrap JS plugins depend on it) -->
    <script src="https://code.jquery.com/jquery-2.1.4.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
  </body>
</html>
