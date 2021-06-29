<!Doctype html>
<html> 
<head>
<title>contact-form-design</title>
<style>
body{
}
form 
{
margin-top: 50px;
transition: all 4s ease-in-out; 
}
.form-control{
width: 600px;
background: transparent;
border: none;
outline: none;
border-bottom: 2px solid green;
color: maroon;
font-size: 35px; 
margin-bottom:20px;
}
input{
height:45px;
} 
form .submit{
background: blue;
border-color: transparent;
color: orange;
font-size: 20px;
font-weight: bold;
letter-spacing: 2px;
height: 50px;
margin-top: 20px;
}
form .submit:hover{
background-color: red;
cursor: pointer;
}

<?php
      $name = $_POST['name'];
      $visitor_email = $_post['email'];
      $message = $_POST['message']

      $email_from = ' kuileyshi3000k@gmail.com';
      
      $email_subject = "new form submission";
      
      $email_body = "User name: $name.\n."
                      "User Email: $visitor_email.\n."
                        "User message: $message.\n";

     $to = "kuileyshi3000k@gmail.com";
     $header ="from: $email_from \r\n";
$headers .= "reply-to: $visitor_email \r\n";
 mail($to,$email_subject,$email_body,$headers);
    header( " location: index.html");
?>

</...11:24 PM 6/12/2021type php page name<form id="contact-form" method= " post" action= "">this code coz the comp cannot runn the php code...you need to upload
this complete code on your server then it will work ......\>






.contact-title{
margin-top: 100px;
color: blue;
text-transform: uppercase; 
transition: all 4s ease-in-out;
}

</style>
</head>

<body>
<div class= "contact-title">
<h1><em>any heater,all solutions<em></h1>
<h2><em>get faster and simple solutions<em></h2>

<div class="contact-form">
<form id="contact-form" method= " post" action= "contact-form-handler.php">
<input name="name" type="text" class="form-control" placeholder="your name" required><br>
<input name="email" type="email" class="form-control" placeholder="your email" required><br>
<textarea name="message" class="form-control" placeholder= "message" row="7" required></textarea><br>

<input type="submit" class="form-control submit" value="send message">
</form>

</div>

</body>


</html>
get easy solutions
