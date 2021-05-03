# freeswitch-german-soundfiles

German language files for Freeswitch. Conference sound files only -primarily for use with BigBlueButton.

There are two options to use in BBB:


1. Using freeswitch config (thanks to [@sualko]( https://github.com/sualko )):

a. run `mkdir -p /opt/freeswitch/share/freeswitch/sounds/de/de/callie/conference` and upload all folders to this path.
b. edit `/opt/freeswitch/etc/freeswitch/autoload_configs/conference.conf.xml`
        -->      replace `<param name="sound-prefix" value="$${sounds_dir}/en/us/callie"/>` with `<param name="sound-prefix" value="$${sounds_dir}/de/de/callie"/>`
c. restart BBB by using `bbb-conf --restart` from shell

2. Simply replacing all files
 
replace files in `/opt/freeswitch/share/freeswitch/sounds/en/us/callie/conference` with the ones provided here.


3. If you use the docker version from [alangecker/bigbluebutton-docker](https://github.com/alangecker/bigbluebutton-docker) simply add a volume mapping to the following path inside your container:
```
`/usr/share/freeswitch/sounds/en/us/callie/conference`
```

I'm always open for other/better translation suggestions!
