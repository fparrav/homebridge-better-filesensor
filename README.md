# homebridge-better-filesensor

[![npm version](https://badge.fury.io/js/homebridge-better-filesensor.svg)](https://badge.fury.io/js/homebridge-better-filesensor)

Fork de  [SphtKr/homebridge-filesensor](https://github.com/SphtKr/homebridge-filesensor).

# Changelog:
* Parameter is added to detect changes in network drives [ `usePolling: true` ].

Original Readme : 
  


> Is a plugin for [Homebridge](https://github.com/nfarina/homebridge) that uses [Chokidar](https://github.com/paulmillr/chokidar).
> 
> This plugin creates a motion sensor or contact sensor accessory based on watching a directory or file. This is useful because many inexpensive IP cameras (Foscam, D-Link, others) have an option to FTP an image or video file when they detect motion. If you use this accessory to monitor that FTP drop location, you can expose that camera as a motion sensor to HomeKit.
> 
> If you have trouble getting this one working, also check out [homebridge-smtpsensor](https://github.com/sphtkr/homebridge-smtpsensor), which lets you create motion sensors based on email triggers (which many IP cameras can also send).
> 
> Configuration
> 
> | Key | Description |
> | --- | --- |
> | `path` | The directory, file, or glob to watch (see docs for the chokidar module for what's possible) |
> | `window_seconds` | A file modification date has to be within this many seconds of now to trigger the sensor. This is also the length of time that the sensor will stay triggered before falling back to it's default state. |
> | `inverse` | If needed, you can invert the behavior of the sensor, for instance so that finding a file means there is ''no'' motion or contact detected. |
> | `sensor_type` | Currently either "m" for motion sensor or "c" for contact sensor. |
> 
> NOTE: Contact sensor support is a little wonky right now, it doesn't seem to want to fall back to the untriggered state for some reason--also app support seems to be lacking.
