

    nothing of the described above works for me. I just used latest version of destroy windows 10 spying, trying to comment out lines suggested in hosts file, the only line present is # 0.0.0.0 client-s.gateway.messenger.live.com

    Flushing dns and deleting skype folder in appdata doesn't help.

    Could someone elaborate how do I "unlock firewall" and "host: 64.4.23.0-64.4.23.25" like suggested by user above? thanks

    Update: Tried deleting all entries in hosts, to check if it's something blocking in this file, but no, skype still does not connect.

    Update: tried to allow skype in firewall, it is allowed there anyway, tried to enabling/disabling, no use.

    Update: running these commands helped:

    netsh advfirewall firewall delete rule name="157.55.235.0-157.55.235.255_Block"
    netsh advfirewall firewall delete rule name="157.55.56.0-157.55.56.255_Block"
    netsh advfirewall firewall delete rule name="64.4.23.0-64.4.23.255_Block"
    netsh advfirewall firewall delete rule name="65.55.223.0-65.55.223.255_Block"

    uninstall all previous skype versions with revo uninstaller (with cleaning all skype junk)
    open cmd.exe as administrator and run theese 4 commands from comment above
    comment next lines in hosts:
    #0.0.0.0 m.hotmail.com
    #0.0.0.0 client-s.gateway.messenger.live.com
    also ipconfig /flushdns in cmd.exe with administrator rights
    download and install skype from https://www.skype.com/ru/get-skype/
    PROFIT!!!

p.s. some problems can be if your Windows Defender is enabled. If nothing helps, try to disable it, both for private and public networks, and add Skype to acceptable applications for Windows Defender.

# Destroy Windows 10 Spying

### Features
  
- Remove all spyware modules
- Remove spying apps
- Add spying domains to hosts file!
- Remove spying services
- Remove Windows 10 Metro Apps
- Support Windows 7/8/8.1/10 and Server 2008-2012 R2
- Remove Office 2016 telemetry
- Open Source!

### Copyright 2018 RENESSANS LLC

[Twitter @renessans_bz](https://twitter.com/renessans_bz)

### License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  * [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

