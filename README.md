# routetable
Route table creation with subnet association. Cross subscription routing from a spoke to the hub

# Steps

1. Clone repo to local machine
1. Update variables.tf with new values
1. Update main.tf backend details
1. Select service principal and setup azure devops pipeline
1. update yaml file with required group varibles and azure subscription

2. Calling the module;

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