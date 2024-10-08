# Documentation for the GameDriver Unreal API

This documentation is the latest available for the GameDriver test automation SDK for Unreal. For documentation specific to older versions, please refer to support.gamedriver.io or the documentation that shipped with your specific version.

The documentation is divided into the main [ApiClient](https://github.com/GameDriver-io/gdio.unreal_api.doc/blob/master/gdio.unreal_api/ApiClient.md) with shared use of [Common Objects](https://github.com/GameDriver-io/gdio.unity_api.doc/blob/main/gdio.common.objects.md). For more information on usage and general "how-to", please visit [support.gamedriver.io](https://support.gamedriver.io).

You will note there are two sets of KeyCode values:One for Unreal 4.X and another for those using Unreal 5 and greater. Be sure to use the KeyCode and api version that matches your Unreal version or you may experience mapping issues on your inputs (especially in VR). 


For users using Gamedriver with the UnrealAutomation Testing Framework, you can see the api documentation [Unreal Automated Testing GameDriver Api](UnrealTestFramework/Classes/class_u_g_d_i_o_api.md). 

For those using Blueprints in unreal, check out the [Blueprint methods](UnrealTestFramework/Classes/class_u_b_p___g_d_i_o_a_p_i.md)


If you find an issue with this documentation, please let us know in the Issues tab, or by sending an email to support@gamedriver.io

Thank you for choosing GameDriver for your test automation needs!

# Change log

Added new convenience api calls
Added documentation for the new blueprint/C++ Api calls available in V2.1 onwards.
Removed the need to explicitly include UE4 or UE5 namespaces. Use the api that matches your unreal major engine version.
