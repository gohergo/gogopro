
1. secure route TLS Termination: Passthrough

2. use XCA or openssl, sign a certificate for *.1d35.starter-us-east-1.openshiftapps.com, export cert+key.pem

3. docker image: wangyi2005/goproxy-vps, Environment Variables: CONFIG_FILE_URL e.g.https://pastebin.com/raw/ystHQBiU

4. create a pastebin, server_name = ["yourhostname.1d35.starter-us-east-1.openshiftapps.com"], pem from cert+key.pem

5. chrome+SwitchyOmega https proxy:  yourhostname.1d35.starter-us-east-1.openshiftapps.com:443
