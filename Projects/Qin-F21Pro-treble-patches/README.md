# Patch Bluetooth and Headphones

1. Create a folder called bluetooth in vendor / overlay and grant permissions 755

2. Put bluetooth.apk in the folder and give it 644 permissions

3. Create a folder named devinputjack in vendor / overlay and grant permissions 755

4. Add devinputjack to the folder and give it 644 permissions

5. In system / bulid.prop, in the section


#Disable for evryone for the moment

add:
```
persist.sys.overlay.devinputjack = true
persist.sys.phh.disable_a2dp_offload = true
```

And add anter (so that there is a space of one row before the row
#Disable debugging strict mode toats)
thanks to all GSI developers in 4pda.ru on the help&files!

# Add hardware keyboard support
copy /system/usr/keylayout folder from a stock ROM to your GSI ROM
