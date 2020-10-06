# Google Cloud SDK installer

### Gcloud SDK

In the [google cloud site](https://cloud.google.com/sdk/docs/downloads-interactive) you will be able to find all platforms installation guide.
or follow the bellow commands for Linux distribution.

### 1. Linux
##### Request the installer and execute it with bash
```bash
curl https://sdk.cloud.google.com | bash
```
##### Restart your shell
```bash
exec -l $SHELL
```
##### Run gcloud init to initialize the gcloud environment
```bash
gcloud init
```
if last command doesn't work then you might need to re-install and press Y to prompt `Modify profile to update your $PATH and enable bash completion? (Y/n)` or
 update your environment variable $PATH to point also to /PATH-TO-GCLOUD/google-cloud-sdk/bin. [Update $PATH](https://stackabuse.com/how-to-permanently-set-path-in-linux/)
```
export PATH="/$PATH-TO-GCLOUD-DIR/google-cloud-sdk/bin:$PATH"
```


