# OpenSSL-Signing
An easy code to help you create a signature for APIs that require one.


### My variables
$plainText - That's a concatination of different data that was required for the API i was using. <br />
$fp - opens the file that contains my private key. <br />
$privKey - reads the private key. <br />
$privateKey - converts the $privKey to a string. <br />
$token - access token from the API i am using <br />

Then if you do an echo base64_encode($signature); you'll get to see your signature. 
Note: Without the  base64_encode() you'll see gibberish.

### To generate key pair keys
openssl genrsa -out privatekey.pem 2048 -nodes <<<<<<<<<< For linux users and maybe IOS
download keystore explorer or install openssl <<<<<<<<<< For windows but do more research 
