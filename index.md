<html>
<body>
<!-- Just an image -->
<nav class="navbar navbar-light bg-light">
  <a class="navbar-brand" href="#">
    <img src="sawo.png" width="100" height=auto alt="">
  </a>
</nav>
<div>
<div>
  <img src="computer-image.png" width="500" height=auto alt="">
  <p>
    Chat with your closest friends no matter how far they are
  </p>
</div>
<div>
 <div id="sawo-container" style="height: 300px; width: 300px;"></div>
  <p>Login and enjoy</p>
  
</div>
</div>
</div>
<script src="http://websdk.sawolabs.com/sawo.min.js"></script>
        <script>
            var config = {
                containerID: "sawo-container",
                identifierType: "email", // can be either 'email' or 'phone_number_sms'
                apiKey: "d259c813-163d-4f7e-9485-e703ec4c95c1", // add your api key here
                onSuccess: (payload) => {
                    document.getElementById("status").innerHTML =
                        "Login Success";
                },
            };
            var sawo = new Sawo(config);
            sawo.showForm();
        </script>
</body>
</html>
