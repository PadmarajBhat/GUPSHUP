# What is Gupshup?
* it is a layer on the top of whatsapp api
* event.messageobj.type determines the type of the message shared.
  * type == "image" : imageURL is sent
   * image sent gets stored in gupshup file manager
   * there is no access to the root directory even if it is http link to gupshup fm
   * this is same for recived or sent images.
   * persistence of the data is perhaps subjected to enterprise account
* enterprise account takes upto 7 days for approval
* node debugger is launching :(
  * chrome debugger should have launched
* whatsapp processing can take map location and has to be processed under LocationHandler 
   * messageobj.latitude and messageobj.longitude are keys files
* MessageHandler process user inputs
* simpledb.botlevel can be handy to manage multitenancy
* surprisingly, event structure different for different apps that gupshup supports
  * it has whatsapp number and senderName
    * Perhaps name can be same !!!!
* There are 2 types of persistences supported in Gupshup:
  * context.simpledb.botleveldata
    * scope of the data is throughout the life span of bot.
  * context.simpledb.roomleveldata
    * scope of the data is throughout the specific conversation of the user.
* A new bot can be started through 2 imp ways:
  * IDE 
  * flowbuilder
  * in either ways "default.scr" defines the flow direction

* there is debug mode in settings of bot which will let us capture production log
  * however only error logs gets saved: console.err()
  * response to user is automatically saved
  * u need to have JSON.stringify() to get the same in whatsapp or logs
 
* roomlevel has "state"
 * what does it indicate? current or past ?
 * would it matter if it is inside success or when in script handler scope ?
