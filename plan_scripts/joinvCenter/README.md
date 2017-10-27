This is modified version of William Lam's sript from http://www.virtuallyghetto.com/2011/03/how-to-automatically-add-esxi-host-to.html.

#### Many thanks William Lam for his original script.

This is special version of plan script for HPE Image Streamer.

Please use: 
* vCenter-add-60 - for vCenter 6.0;
* vCenter-add-65 - for vCenter 6.5;

You need to use this plan script together with https://github.com/fedorovant/image-streamer-esxi-plan-scripts/blob/master/plan_scripts/httpClient_policy

Just create a copy of original HPE - ESXi - deploy .. build plan from https://github.com/HewlettPackard/image-streamer-esxi/tree/v3.1/artifact-bundles and customize it with this 2 additional steps:
* httpClent plan script;
* one of vCenter-add plan script;
* at your custom build plan change `@vc_password1@` varible type from String to Password type.

I'll add wiki page with step-by-step guide at near future.
