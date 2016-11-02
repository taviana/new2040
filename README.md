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
        
        $.ajax({
          url: "http://challenge.code2040.org/api/register",
          type: 'POST',
          crossDomain: true,
          dataType: 'text',
          data: JSON.stringify(send)
          }).done(function (data){
            $(".container").text(data);
            console.log(data);
            });
      });
      </script>
  </body>
</html>

