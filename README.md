# new2040
<!DOCTYPE html>
  <body>
  
    <div class = "keys">
    </div>
    <script>
      var send = {
        "token" = "cd61a19c72bc0773bc933a70edde8d1f",
        "github" = "https://github.com/taviana/new2040"
      }
      
      $(document).ready(function(){
        $(".keys").text("ready!");
        $(".keys").text(send);
        console.log(send);
        
        $.post("http://challenge.code2040.org/api/register")
      });
      </script>
  </body>
</html>

