## HTML
- Hyper Text Markup Language
- used to structure a web page
- Sample Code: -
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Title of the webpage</title>
  </head>
  <!-- <tagname style="property:value;"> -->
  <body style="background-color:powderblue;">
    <h1 id="top" style="border:2px solid Tomato;">Heading</h1>
    <p>Paragraph 1<br><!-- Empty HTML Element -->Paragraph 2</p>
    <hr>
    <p style="color:red; font-family:courier; font-size:300%; text-align:center;" title="I'm a tooltip">A Paragraph.</p>
    <img src="/relative/url/created.jpg" alt="Alternate Text" height="500" width="500"><!-- preferred to use style over here like this style:"height:40px;width:40px;" -->
    <!-- Preformatted text -->
    <pre>Preformatted text sample
    This is line 1.
    This is line 2.</pre>
    <!-- Text Formatting -->
    <p><b><i>Hello There<sup>!!!</sup></i></b></p>
    <p><strong><em>Just</em> to <ins>show</ins></strong></p>
    <p><small>various</small> <del>a</del> <mark>text formatting</mark><sub>...</sub></p>
    <h2>HTML Links</h2>
    <h3>Absolute Links</h3>
    <p><a href="https://www.google.com/" title="Go to Google" target="_blank">Google</a></p>
    <p><a href="mailto:someone@example.com">Send email</a></p>
    <button onclick="document.location='default.php'">Button</button>
    <a href="#top">Jump to Top</a>
  </body>
</html>


## HTML Tables
<!DOCTYPE html>
<html>
  <head>
    <style>
      table, th, td{border: 1px solid black;
                    border-radius: 10px;
                    <!-- To avoid double borders, use:-border-collapse: collapse; -->
                    border-style:outset;
                    border-color: red;}
      th, td{background-color: cyan; padding: 15px; border-spacing: 30px}
      tr:nth-child(even) {background-color: blue;}
      th:nth-child(even), td:nth-child(even) {background-color: red;}
    </style>
  </head>
<body>
  <table>
    <caption>Employees' Details</caption>
    <tr>
      <th style="width:50%" text-align: center;>Serial Number</th>
      <th colspan="2">Name</th>
      <th>Company</th>
      <th>City</th>
      <th>Country</th>
    </tr>
    <tr style="height:70%">
      <th>1</th>
      <td>Adam</td>
      <td>Smith</td>
      <td>Google</td>
      <td>New York City</td>
      <td>USA</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Eve</td>
      <td>Jackson</td>
      <td>Meta</td>
      <td>London</td>
      <td>UK</td>
    </tr>
  </table>
</body>
</html>
