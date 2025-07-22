#  Azure Policy definitions for Azure Native Dynatrace Service samples
### about
sample Azure Policy definitions that ensures Diagnostic Settings are created

assumptions:
* it should be possible to re-fine enabled log categories, to optimize cost
* Policy can be assigned to `management group` or `subscription` 
* Policy OOTB provides a way to filter out resource groups, and individual instances
* location is addition Policy parameter for filtering resources 
* (TO-DO) consider adding tag-filtering expression
* `DynatraceMonitoringPolicyRole` is a least privilege role, that allows to create Diagnostic Settings pointing to Azure Native Dynatrace Service. Build-in roles are not sufficent (contributor or owner role will be required.)

todo:
* fix the selection conditions for both policies