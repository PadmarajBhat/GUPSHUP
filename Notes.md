# What is Gupshup?
* it is a layer on the top of whatsapp api
* event.messageobj.type determines the type of the message shared.
  * type == "image" : imageURL is sent
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
