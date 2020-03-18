# routetable
Route table creation with subnet association. Cross subscription routing from a spoke to the hub

# Use

2. Calling the module;

```terraform
module "create" {
    source                  = "github.com/ukho/tfmodule-azure-routetable-hub-spoke"
    spokesubscriptionid     =  var.spokesubscriptionid
    hubsubscriptionid       =  var.hubsubscriptionid
    spokerg                 =  var.spokerg
    hubrg                   =  var.hubrg
    hubrt                   =  var.hubrt
    id                      =  var.id
    routetable              =  var.routetable
    routeaddress            =  var.routeaddress
    route                   =  var.route
    hop                     =  var.hop
    api                     =  var.api
    nsb                     =  var.nsb
    web                     =  var.web
    hubprefix               =  var.hubprefix
    spokeprefix             =  var.spokeprefix 
}
```
