All executables must have at least these two entitlements:

<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
    <key>platform-application</key>
    <true/>
    <key>com.apple.private.security.container-required</key>
    <false/>
</dict>
</plist>
Tweaks and stuff get installed in: /var/containers/Bundle/tweaksupport the same way you did with Electra betas.
Tweaks must be patched using the patcher script provided. (Mac/Linux/iOS only) or manually with a hex editor
Apps get installed in /var/Apps and later you need to run /var/containers/Bundle/iosbinpack64/usr/bin/uicache (other uicache binaries won't work)
