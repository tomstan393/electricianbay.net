# electricianbay.net

<!DOCTYPE html>
<html>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
	<link rel="stylesheet" type="text/css" href="myStyle.css" >
    <body>
	    

       		<div class="login-wrap">
		    <div class="login-html">
		        
		    
			 <input id="tab-1" type="radio" name="tab" class="sign-in" checked><label for="tab-1" class="tab">SIGN IN</label>
			    <input id="tab-2" type="radio" name="tab" class="sign-up"><label for="tab-2" class="tab">SIGN UP</label>
		
        		    <div class="login-form">
        		        
        		        
        		        
        			    <div class="sign-in-htm">
        			        
        			        <form action="action_page.php" method="post" onsubmit="return checkForm_Sign_In(this)">
        			            
                				    <div class="group">
                					    <label for="user" class="label">Username</label>
                					    <input id="user" type="text" class="input" name="username" required size="32">
                				    </div>
                    				    
                    				<div class="group">
                    					<label for="password" class="label">Password</label>
                    					<input id="password" type="password" class="input" data-type="password" name="password" required size="32">
                    				</div>
                    				
            				        
            				        <div class="group">
            					        <input type="submit" class="button" value="Sign In">
            				        </div>
            				        
                				    <div class="hr"></div>
                				    
                				    
                    			     <div class="foot-lnk">
                    					<a href="forgot_password.html">Forgot Password?</a>
                    				</div>
                    				
                    				<script>
    
                                              function checkForm_Sign_In(form)
                                              {
                                                    /*var re = /^[]+$/;
                                                    
                                                    
                                                    if(!re.test(form.username.value)) 
                                                    {
                                                    alert("Error: Username contains one of invalid characters: /,^,[,],+,$,\\");
                                                          form.username.focus();
                                                          return false;
                                                    }
                                                    else if(!re.test(form.password.value)) 
                                                    {
                                                    alert("Error: Password contains one of invalid characters: /,^,[,],+,$,\\");
                                                          form.password.focus();
                                                          return false;
                                                    }*/
                                               
                                                return true;
                                              }

                                     </script>
         			
                    		</form>
    			</div>
    			
    			<div class="sign-up-htm">
    			    
    			      <form action="registration.php" method="post" onsubmit="return checkForm_Sign_Up(this)">
    				
                				<div class="group">
                					<label for="new_username" class="label">Username</label> 
                					<input id="new_username" type="text" class="input" name="new_username" required size="32">
                				</div>
                			
                			    <div class="group">
                					<label for="new_password" class="label">Password (at least 8 characters)
                					    <input id="new_password" type="password" class="input" data-type="password" name="new_password" required size="32" minlength="8" onkeyup='check();'>
                					</label>
                				</div>
                				
                				<div class="group">
                					<label for="confirm_password"  class="label">Repeat Password 
                    					<input id="confirm_password" type="password" class="input" data-type="password" 
                					        name="confirm_password" required size="32" onkeyup='check();'>
                					        <span id='message'></span>
                					</label>
        					       
                				</div>
                				
                				<div class="group">
                					<label for="email" class="label">Email Address</label>
                					<input id="email" type="text" class="input" name="email" required size="32">
                				</div>
                				
                				<div class="group">
                					<input type="submit" name="submit" class="button" value="Sign Up">
                				</div>
                				
                				<div class="hr">
                				    
                				</div>
                				
                				<div class="foot-lnk">
                					<label for="tab-1">Already Member?</label>
                			
                		       </div>
                		       
                		       
                		   
                		<script>
                                        
                                         function checkForm_Sign_Up(form)
                                          {
                                              
                                                /*var re = /^[\w ]+$/;
                                                
                                                
                                                if(!re.test(form.new_username.value)) 
                                                {
                                                      alert("Error: Username contains one of invalid characters: /,^,[,],+,$,\\" );
                                                      form.new_username.focus();
                                                      return false;
                                                }
                                                else if(!re.test(form.new_password.value)) 
                                                {
                                                      alert("Error: Password contains one of invalid characters: /,^,[,],+,$,\\");
                                                      form.new_password.focus();
                                                      return false;
                                                }
                                               
                                                else if(!re.test(form.email.value)) 
                                                {
                                                      alert("Error: Email contains one of invalid characters: /,^,[,],+,$,\\");
                                                      return false;
                                                }
                                                else */if (form.new_password.value.localeCompare(form.confirm_password.value) != 0)
                                                {
                                                     alert("Error: Password not matching");
                                                     form.new_password.focus();
                                                     return false;
                                                }
                                               
                                                return true;
                                             
                                          }
              
        				                var check = function() 
        				                {
                                              if (document.getElementById('new_password').value ==
                                                document.getElementById('confirm_password').value) 
                                              {
                                                document.getElementById('message').style.color = 'green';
                                                document.getElementById('message').innerHTML = 'password matching';
                                              } else 
                                              {
                                                document.getElementById('message').style.color = 'red';
                                                document.getElementById('message').innerHTML = 'password not matching';
                                              }
                                        }
              
                			  </script>
                	   </form>
    	        </div>
            </div>  
        </div> 
        </div> 
  

    </body>
</html>
