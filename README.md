# file1.html
<html>
  <head>
    <title>Form Validation</title>
    <script>
      function validateform(){
      var firstname=document.myform.fname.value;
      var lastname=document.myform.lname.value;
      var email=document.myform.email.value;
      
      if(firstname==null || firstname==""){
      alert("Name can't be blank");
      return false;
      }else if(lastname.length<6){
      alert("Last name must be 6 char long");
      return false;
      }
      }
      </script>
      <body>
      <form name="myform" method="post"action="abc.jsp" onsubmit="return validateform()">
      First name:<input type="text" name="fname"><br/>
      Last name:<input type="text" name="lname"><br/>
      Email address:<input type="text" name="email"><br/>
      Branch <select name="branch">
      <option>Computer Science
      <option>Information Technology
      </select>
      <input type="submit" value="register">
      </form>
      </body>
      </html>
      
      
