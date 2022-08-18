# ZenDeskUpload
An upload method with sharex to upload to any website that uses ZenDesk


## How to upload to any website that uses Zen Desk

### Example Websites: 
https://en.help.roblox.com
https://support.discordapp.com
https://help.pornhub.com
https://help.minecraft.net
https://consumercomplaints.fcc.gov
https://faqs.in.gov
https://support.zoom.us
https://support.virustotal.com
https://support.aminoapps.com
https://help.iheart.com
https://support.nzxt.com
https://support.udemy.com
https://consumercomplaints.fcc.gov

and put this in a sharex file

```
{
  "Version": "13.1.0",
  "Name": "zendeskuploader",
  "DestinationType": "ImageUploader, TextUploader, FileUploader",
  "RequestMethod": "POST",
  "RequestURL": "[domain]/api/v2/uploads.json",
  "Parameters": {
    "filename": "$filename$"
  },
  "Body": "Binary",
  "URL": "$json:upload.attachments[0].mapped_content_url$"
}
```
Replace [domain] with any domain that uses Zen Desk
