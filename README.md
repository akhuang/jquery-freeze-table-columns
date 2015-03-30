jquery-freeze-table-columns
===========================

A JQuery plugin to freeze table columns and headers written by Conan Albrecht

Original post: http://warp.byu.edu/site/content/1020
Usage example:  http://eureka.ykyuen.info/2013/04/08/jquery-freeze-html-table-header-and-the-left-columns




=======
<!DOCTYPE html>
<html>
  <head>
  <meta charset="UTF-8" />
  <style type="text/css">
    body {
      margin: 0px auto;
      width: 800px;
    }
    #freeze-table {
      width: 1200px;
    }
    th {
      background-color: grey;
    }
  </style>
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
  <script src="jquery.freezetablecolumns.1.1.js"></script>
  <script type="text/javascript">
    $(document).ready(function(){
      $('#freeze-table').freezeTableColumns({
        width:       800,   // required
        height:      500,   // required
        numFrozen:   2,     // optional
        frozenWidth: 160,   // optional
        clearWidths: true,  // optional
      });
    });
  </script>
  </head>
  <body>
    <table id="freeze-table">
      <tr>
        <th>Name</th>
        <th>Location</th>
        <th>Registration Date</th>
        <th>Occupation</th>
        <th>Profession</th>
        <th>Registration Date</th>
        <th>Occupation</th>
        <th>Profession</th>
      </tr>
      <tr>
        <td>Kit</td>
        <td>Hong Kong</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
      </tr>
      <tr>
        <td>Kit</td>
        <td>Hong Kong</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
      </tr>
      <tr>
        <td>Kit</td>
        <td>Hong Kong</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
        <td>2013-04-08</td>
        <td>Freelancer</td>
        <td>Web development</td>
      </tr>
    </table>
  </body>
</html>
