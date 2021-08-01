# mysql-dropbox-backup

Dump MySQL databases, compress them, and upload to [Dropbox] for a simple off-site backup. Backups are kept for 14 (customiseable) days.

# Requirements

* cURL
* A [Dropbox] account

# Usage

## Dropbox account setup
1. Go to [developers.dropbox.com](https://developers.dropbox.com) and create an App, copy the App key & secret.
2. Now go to App permissions and check `files.metadata.write` and `files.content.write` and save.

## Database credentials
1. Edit `mysql-dropbox-backup.cnf` file to add Database connection details. 

## Run
1. In the terminal, run `./mysql-dropbox-backup.sh`
2. Enter App Key
3. Enter App Secret Key
4. Click on the generated link
5. Click continue
6. Copy the code from browser and paste into terminal
7. Type `y` and hit *Enter*
8. The files should get uploaded to the root directory in Dropbox (You can edit `dropbox_uploader.sh` to put the files in a subfolder on Dropbox.)