[Back to the Ling/Light_Kit_Admin_TaskScheduler api](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler.md)



The LightKitAdminTaskSchedulerService class
================
2020-07-31 --> 2020-08-07






Introduction
============

The LightKitAdminTaskSchedulerService class.



Class synopsis
==============


class <span class="pl-k">LightKitAdminTaskSchedulerService</span> extends [LightLingStandardServiceKitAdminPlugin](https://github.com/lingtalfi/Light_LingStandardService/blob/master/doc/api/Ling/Light_LingStandardService/Service/LightLingStandardServiceKitAdminPlugin.md) implements [LightRealistCustomServiceInterface](https://github.com/lingtalfi/Light_Realist/blob/master/doc/api/Ling/Light_Realist/Service/LightRealistCustomServiceInterface.md), [PluginInstallerInterface](https://github.com/lingtalfi/Light_PluginInstaller/blob/master/doc/api/Ling/Light_PluginInstaller/PluginInstaller/PluginInstallerInterface.md) {

- Inherited properties
    - protected [Ling\Light\ServiceContainer\LightServiceContainerInterface](https://github.com/lingtalfi/Light/blob/master/doc/api/Ling/Light/ServiceContainer/LightServiceContainerInterface.md) [LightLingStandardServiceKitAdminPlugin::$container](#property-container) ;
    - protected array [LightLingStandardServiceKitAdminPlugin::$options](#property-options) ;

- Inherited methods
    - public LightLingStandardServiceKitAdminPlugin::__construct() : void
    - public LightLingStandardServiceKitAdminPlugin::setContainer([Ling\Light\ServiceContainer\LightServiceContainerInterface](https://github.com/lingtalfi/Light/blob/master/doc/api/Ling/Light/ServiceContainer/LightServiceContainerInterface.md) $container) : void
    - public LightLingStandardServiceKitAdminPlugin::setOptions(array $options) : void
    - public LightLingStandardServiceKitAdminPlugin::install() : void
    - public LightLingStandardServiceKitAdminPlugin::isInstalled() : bool
    - public LightLingStandardServiceKitAdminPlugin::uninstall() : void
    - public LightLingStandardServiceKitAdminPlugin::getDependencies() : array
    - public LightLingStandardServiceKitAdminPlugin::registerByRequestId(string $requestId) : mixed | void
    - protected LightLingStandardServiceKitAdminPlugin::error(string $msg) : void
    - private LightLingStandardServiceKitAdminPlugin::prepareTheNames() : void

}






Methods
==============

- LightLingStandardServiceKitAdminPlugin::__construct &ndash; Builds the LightLingStandardService01 instance.
- LightLingStandardServiceKitAdminPlugin::setContainer &ndash; Sets the container.
- LightLingStandardServiceKitAdminPlugin::setOptions &ndash; Sets the options.
- LightLingStandardServiceKitAdminPlugin::install &ndash; Installs the plugin in the light application.
- LightLingStandardServiceKitAdminPlugin::isInstalled &ndash; Returns whether the core install phase of the plugin is fully completed.
- LightLingStandardServiceKitAdminPlugin::uninstall &ndash; Uninstalls the plugin.
- LightLingStandardServiceKitAdminPlugin::getDependencies &ndash; Returns the array of dependencies.
- LightLingStandardServiceKitAdminPlugin::registerByRequestId &ndash; Registers the plugin dynamically to [the realist plugin](https://github.com/lingtalfi/Light_Realist/).
- LightLingStandardServiceKitAdminPlugin::error &ndash; Throws an exception.
- LightLingStandardServiceKitAdminPlugin::prepareTheNames &ndash; prepareTheNames names used by this class.





Location
=============
Ling\Light_Kit_Admin_TaskScheduler\Service\LightKitAdminTaskSchedulerService<br>
See the source code of [Ling\Light_Kit_Admin_TaskScheduler\Service\LightKitAdminTaskSchedulerService](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/Service/LightKitAdminTaskSchedulerService.php)



SeeAlso
==============
Previous class: [LightKitAdminTaskSchedulerLkaPlugin](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/LightKitAdminPlugin/Generated/LightKitAdminTaskSchedulerLkaPlugin.md)<br>
