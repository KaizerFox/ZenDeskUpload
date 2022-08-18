# ZenDeskUpload
An upload method with sharex to upload to any website that uses ZenDesk


## How to upload to any website that uses Zen Desk

### Example Websites: 
https://en.help.roblox.com <br>
https://support.discordapp.com <br>
https://help.pornhub.com <br>
https://help.minecraft.net <br>
https://consumercomplaints.fcc.gov <br>
https://faqs.in.gov <br>
https://support.zoom.us <br>
https://support.virustotal.com <br>
https://support.aminoapps.com <br>
https://help.iheart.com <br>
https://support.nzxt.com <br>
https://support.udemy.com <br>
https://consumercomplaints.fcc.gov <br>
<br>

and put this in a sharex (sxcu) file

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
