Light_Kit_Admin_TaskScheduler
===========
2020-07-31



A [Light Kit Admin](https://github.com/lingtalfi/Light_Kit_Admin) wrapper for the [Light_TaskScheduler](https://github.com/lingtalfi/Light_TaskScheduler) plugin.




This is a [Light plugin](https://github.com/lingtalfi/Light/blob/master/doc/pages/plugin.md).

This is part of the [universe framework](https://github.com/karayabin/universe-snapshot).


Install
==========
Using the [uni](https://github.com/lingtalfi/universe-naive-importer) command.
```bash
uni import Ling/Light_Kit_Admin_TaskScheduler
```

Or just download it and place it where you want otherwise.






Summary
===========
- [Light_Kit_Admin_TaskScheduler api](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler.md) (generated with [DocTools](https://github.com/lingtalfi/DocTools))
- [Conception notes](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/pages/conception-notes.md)
- [Services](#services)






Services
=========


Here is an example of the service configuration:

```yaml
kit_admin_task_scheduler:
    instance: Ling\Light_Kit_Admin_TaskScheduler\Service\LightKitAdminTaskSchedulerService
    methods:
        setContainer:
            container: @container()




# --------------------------------------
# hooks
# --------------------------------------
$bmenu.methods_collection:
    -
        method: addDefaultItemByFile
        args:
            menu_type: admin_main_menu
            file: ${app_dir}/config/data/Light_Kit_Admin_TaskScheduler/bmenu/generated/kit_admin_task_scheduler.admin_mainmenu_1.byml

$chloroform_extension.methods_collection:
    -
        method: registerTableListConfigurationHandler
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            handler:
                instance: Ling\Light_Kit_Admin\ChloroformExtension\LightKitAdminTableListConfigurationHandler
                methods:
                    setConfigurationFile:
                        files:
                            - ${app_dir}/config/data/Light_Kit_Admin_TaskScheduler/Light_ChloroformExtension/generated/kit_admin_task_scheduler.table_list.byml



$controller_hub.methods_collection:
    -
        method: registerHandler
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            handler:
                instance: Ling\Light_Kit_Admin_TaskScheduler\ControllerHub\Generated\LightKitAdminTaskSchedulerControllerHubHandler
                methods:
                    setContainer:
                        container: @container()

$crud.methods_collection:
    -
        method: registerHandler
        args:
            pluginId: Light_Kit_Admin_TaskScheduler
            handler:
                instance: Ling\Light_Kit_Admin\Crud\CrudRequestHandler\LightKitAdminCrudRequestHandler

$kit_admin.methods_collection:
    -
        method: registerPlugin
        args:
            pluginName: Light_Kit_Admin_TaskScheduler
            plugin:
                instance: Ling\Light_Kit_Admin_TaskScheduler\LightKitAdminPlugin\Generated\LightKitAdminTaskSchedulerLkaPlugin
                methods:
                    setOptionsFile:
                        file: ${app_dir}/config/data/Light_Kit_Admin_TaskScheduler/Light_Kit_Admin/lka-options.generated.byml

$micro_permission.methods_collection:
    -
        method: registerMicroPermissionsByProfile
        args:
            file: ${app_dir}/config/data/Light_Kit_Admin_TaskScheduler/Light_MicroPermission/kit_admin_task_scheduler.profile.generated.byml


$plugin_installer.methods_collection:
    -
        method: registerPlugin
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            installer: @service(kit_admin_task_scheduler)



$realform.methods_collection:
    -
        method: registerFormHandler
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            handler:
                instance: Ling\Light_Kit_Admin\Realform\Handler\LightKitAdminRealformHandler
                methods:
                    setConfDir:
                        dir: ${app_dir}/config/data/Light_Kit_Admin_TaskScheduler/Light_Realform

$realist.methods_collection:
    -
        method: registerListRenderer
        args:
            identifier: Light_Kit_Admin_TaskScheduler
            renderer:
                instance: Ling\Light_Kit_Admin\Realist\Rendering\LightKitAdminRealistListRenderer
    -
        method: registerRealistRowsRenderer
        args:
            identifier: Light_Kit_Admin_TaskScheduler
            renderer:
                instance: Ling\Light_Kit_Admin\Realist\Rendering\LightKitAdminRealistRowsRenderer
    -
        method: registerActionHandler
        args:
            renderer:
                instance: Ling\Light_Kit_Admin\Realist\ActionHandler\LightKitAdminRealistActionHandler
    -
        method: registerListActionHandler
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            renderer:
                instance: Ling\Light_Kit_Admin\Realist\ListActionHandler\LightKitAdminListActionHandler
    -
        method: registerListGeneralActionHandler
        args:
            plugin: Light_Kit_Admin_TaskScheduler
            renderer:
                instance: Ling\Light_Kit_Admin\Realist\ListGeneralActionHandler\LightKitAdminListGeneralActionHandler


```



History Log
=============

- 1.0.0 -- 2020-07-31

    - initial commit