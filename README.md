<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web-to-Lead Form</title>
    <link rel="stylesheet" href="Index.css">
    <script src="Index.js"></script>
</head>
<body>    
    
    <h1>Create Lead</h1>
    <form action="https://webto.salesforce.com/servlet/servlet.WebToLead?encoding=UTF-8&orgId=00D5j00000B8uzM" 
    method="POST"
    onsubmit="beforeSubmit()"
    >
    
    <input type=hidden name="oid" value="00D5j00000B8uzM">
    <input type=hidden name="retURL" value="http://google.com">
    <input type=hidden name="Lead_Date__c" class="outputdate">   
   
    
    <label for="first_name">First Name</label><input  id="first_name" maxlength="40" name="first_name" size="20" type="text" required="true"/><br>
    
    <label for="last_name">Last Name</label><input  id="last_name" maxlength="80" name="last_name" size="20" type="text" required="true"/><br>
    
    <label for="email">Email</label><input  id="email" maxlength="80" name="email" size="20" type="text" required="true"/><br>
    
    <!-- Lead Date:<span class="dateInput dateOnlyInput"><input  id="00NJ4000003Xrbj" name="00NJ4000003Xrbj" size="12" type="text" /></span><br>
     -->
    <label for="email">Lead Date</label><input id="leadDate" type="date" required="true" class="inputdate"/><br>
    <input type="submit" name="submit" class="submit" />
    
    </form>
</body>
</html>
