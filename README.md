This a homemade voice_pack for DREAME vacuums. Tested un L40 Ultra AE
I based the voice_pack on the files of the GLADOS voice_pack by czaky https://github.com/czaky/dreame_voice_pack/tree/master

Generated random phrases with: https://www.101soundboards.com/tts/720439-gandalf-hifi-tts-computer-ai-voice#goog_rewarded
Edited mp3 with https://www.audacityteam.org/ and exported as *.ogg
Replaced some with Gandalf and left the others from glados for less used phrases for me!


Terminal commands on mac:
zip file -> tar czf voice_pack.tar.gz *.ogg
file size -> ls -l voice_pack.tar.gz 
hash -> md5sum voice_pack.tar.gz 

Imported via Home Assistant integration!  -> https://github.com/Tasshack/dreame-vacuum
RUNS ON ORIGINAL FIRMWARE!!! NO CFW!

Navigate in HA: Go to Developer Tools > Services in Home Assistant.Call Service: Select dreame_vacuum.vacuum_install_voice_pack as the service.Enter Data (YAML Mode): Switch to YAML mode and use the following format:yamlservice: dreame_vacuum.vacuum_install_voice_pack
data:
  entity_id: vacuum.your_dreame_vacuum # Change to your actual entity ID
  lang_id: "EN" # Or custom language code
  url: "https://tar.gz"
  md5: "your_file_md5_hash"
  size: 1234567 # File size in bytes

for this file:
18835611 bytes
9e2a3256efef121cd388d2c6e952617d md5sum
