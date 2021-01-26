<!DOCTYPE html>
<html>

<head>
  <title>Our Company</title>
</head>

<body>

  <h1>Welcome to Our Company</h1> 
  <h2>Web Site Main Ingredients:</h2>

  <p>Pages (HTML)</p>
  <p>Style Sheets (CSS)</p>
  <p>Computer Code (JavaScript)</p>
  <p>Live Data (Files and Databases)</p>
  <div id="webchat"></div> 
  <script src="https://cdn.jsdelivr.net/npm/rasa-webchat/lib/index.min.js"></script>
 
  <script>   
  WebChat.default.init({     
  selector: "#webchat",     
  initPayload: "/get_started",     
  customData: {"language": "en"}, // arbitrary custom data. Stay minimal as this will be added to the socket     
  socketUrl: "http://localhost:5500",     
  socketPath: "/socket.io/",     
  title: "Title",     
  subtitle: "Subtitle",     
  params: {"storage": "session"} // can be set to "local"  or "session". details in storage section.   
  }) 
  </script>
</body>

</html> 
