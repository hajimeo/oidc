### Example command to start
```
curl -o "./oidcserver" -L "https://github.com/hajimeo/samples/raw/master/misc/oidcserver_$(uname)_$(uname -m)" --compressed
chmod u+x ./oidcserver

# Callback URLs for Nexus 3 and the example client app
REDIRECT_URI='http://localhost:8081/oidc/callback?hash=#browse/welcome,http://localhost:9999/auth/callback' ./oidcserver
```

### How to build
https://github.com/hajimeo/samples/blob/096e79309d9f21c8ccdde18687c21973798849bc/runcom/bash_aliases.sh#L793-L837
```
goBuild "" "oidcserver"
```