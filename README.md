# Running on Jenkins

## Workaround
- Image `jenkins/blueocean` is based on Alpine.
- If you use the Jenkins "Go" wrapper-plugin, the downloaded version will not run on Alpine, since it's dynamically linked to libraries that don't exist in Alpine
- Install `apk add libc6-compat` for compatibility
