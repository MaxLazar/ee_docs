### {exp:qr_code}
	
	<img src="{exp:qr_code type="" action="" tel="" data="ExpressionEngine" title="" email="" subj=""}" alt="QR code"/> 

#### Parameters ####
`action = ""` (*optional*)

Plugin has a couple pattern for QR code messages:
  • sms - send sms
  • tel - phone number
  • email - send email
  • bm - add to bookmarks
  • site - addtional data urlencode

`tel = "555-5555"` *required for action type sms,tel*

`email = "name@name.com"` *required for action type email*

`subj = "John Doe"` *required for action type email*
subject for email

`title = "My WebSite"` *required for action type bookmarks* 
Title for bookmark

`size = "4"` *optional, default "4" *
module size

`ecc = "M"` *optional, default M*
ECC level L or M or Q or H

`data = ""` 
default data for encoding

`px_color = "000000"` *optional, default 000000*
pixel color

`bk_color = "ffffff"` *optional, default ffffff*
background color

`outline_size = "2"` *optional, default 2*
outline size

`base_path` 
**path** to web root (required if you use base_cache parameter)

`base_cache` *optional, default "/images/cache/"*
**path** to image folder