# dotsettings

### secrets
make sure you have a .settings dir with the following:
 * home_pass.secret
 * work_pass.secret

### login script
make sure that in ~/Library/LaunchAgents you have the following:
 * com.user.loginscript.plist

### my symlinks:
 * ln -s ~/git/secrets ~/.secrets
 * ln -s ~/git/dotsettings/com.user.loginscript.plist ~/Library/LaunchAgents/com.user.loginscript.plist

### misc commands:
 * launchctl load ~/Library/LaunchAgents/com.user.loginscript.plist
 * launchctl list | grep customlogin
 * tail -f /var/log/system.log
