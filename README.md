# routetable Hub to Spoke

Route table creation with subnet association. Cross subscription routing from a spoke to the hub

## Use

Calling the module:

```terraform
module "create" {
    source                  = "github.com/ukho/tfmodule-azure-routetable-hub-spoke-one-subnet"
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
    subnet_one              =  var.subnet_one
    hubprefix               =  var.hubprefix
    spokeprefix             =  var.spokeprefix
}
```
