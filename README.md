Claromentis Welcome Message
===================

This is a simple JavaScript function that generates a welcome approproiate to the time of day. It uses Claromentis localisation keys allowing for localisation support.

Usage:

Simply add the following function to your JavaScript and insert, or call accordingly.

```javascript

	 function greet() {
	   var houris = (new Date()).getHours();
	   document.write( ( houris>18 ? lmsg('main.intranethome.good_evening') : ( houris>12 ? lmsg('main.intranethome.good_afternoon') : lmsg('main.intranethome.good_morning') ) ) );
	 };

```

Example Implementation:

```html

    <p class="welcome-message">
    		<component class="Claromentis\Core\Widget\JSLocalize" keys="main.intranethome.good_afternoon, main.intranethome.good_morning">
		<script type="text/javascript">
    		greet();
		</script>
        <a href="/intranet/people/myprofile.php"> <txt name="infobar_logged_on_as"> Firstname Lastname</txt></a>, welcome to Connect.
    </p>

```

Enjoy!
