[Back to the Ling/Light_Kit_Admin_TaskScheduler api](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler.md)



The RealGenController class
================
2020-07-31 --> 2020-07-31






Introduction
============

The RealGenController class.



Class synopsis
==============


abstract class <span class="pl-k">RealGenController</span> extends AdminPageController implements LightAwareInterface, LightControllerInterface, RouteAwareControllerInterface {

- Properties
    - protected string [$iframeSignal](#property-iframeSignal) ;

- Inherited properties
    - protected array [LightKitAdminController::$route](#property-route) ;
    - protected Ling\Light\Core\Light [LightController::$light](#property-light) ;

- Methods
    - public [__construct](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/__construct.md)() : void
    - public [render](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/render.md)() : string | Ling\Light\Http\HttpResponseInterface
    - protected [processForm](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/processForm.md)(string $realformIdentifier, string $table, ?array $options = []) : Ling\Chloroform\Form\Chloroform | Ling\Light\Http\HttpResponseInterface
    - public [setOnSuccessIframeSignal](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/setOnSuccessIframeSignal.md)(string $iframeSignal) : void

- Inherited methods
    - public AdminPageController::renderAdminPage(string $page, ?$params = [], ?Ling\Light_Kit\PageConfigurationUpdator\PageConfUpdator $updator = null) : Ling\Light\Http\HttpResponseInterface
    - public LightKitAdminController::setRoute(array $route) : void
    - protected LightKitAdminController::getKitAdmin() : Ling\Light_Kit_Admin\Service\LightKitAdminService
    - protected LightKitAdminController::getFlasher() : Ling\Light_Flasher\Service\LightFlasherService
    - protected LightKitAdminController::getUser() : Ling\Light_User\LightWebsiteUser
    - public LightKitAdminController::renderPage(string $page, ?array $dynamicVariables = [], ?Ling\Light_Kit\PageConfigurationUpdator\PageConfUpdator $updator = null) : Ling\Light\Http\HttpResponseInterface
    - protected LightKitAdminController::getRedirectResponseByRoute(string $route, ?array $urlParams = []) : Ling\Light\Http\HttpRedirectResponse
    - protected LightKitAdminController::checkRight(string $right) : Ling\Light\Http\HttpResponseInterface | null
    - protected LightKitAdminController::checkMicroPermission(string $microPermission) : void
    - protected LightKitAdminController::error(string $msg) : void
    - public LightController::setLight(Ling\Light\Core\Light $light) : void
    - protected LightController::getLight() : Ling\Light\Core\Light
    - protected LightController::getContainer() : Ling\Light\ServiceContainer\LightServiceContainerInterface
    - protected LightController::getHttpRequest() : Ling\Light\Http\HttpRequestInterface
    - protected LightController::hasService(string $serviceName) : bool

}




Properties
=============

- <span id="property-iframeSignal"><b>iframeSignal</b></span>

    This property holds the iframeSignal for this instance.
    
    

- <span id="property-route"><b>route</b></span>

    This property holds the route for this instance.
    See the route page for more information.
    
    

- <span id="property-light"><b>light</b></span>

    This property holds the light for this instance.
    
    



Methods
==============

- [RealGenController::__construct](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/__construct.md) &ndash; Builds the instance.
- [RealGenController::render](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/render.md) &ndash; Renders a page to interact with a table data.
- [RealGenController::processForm](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/processForm.md) &ndash; or a response directly.
- [RealGenController::setOnSuccessIframeSignal](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/Base/RealGenController/setOnSuccessIframeSignal.md) &ndash; Sets the iframeSignal to use in case of a valid form.
- AdminPageController::renderAdminPage &ndash; if she is not connected yet.
- LightKitAdminController::setRoute &ndash; Sets the matching route to this controller instance.
- LightKitAdminController::getKitAdmin &ndash; Returns the kit admin service instance.
- LightKitAdminController::getFlasher &ndash; Returns a flasher instance.
- LightKitAdminController::getUser &ndash; Returns the current user.
- LightKitAdminController::renderPage &ndash; Renders the given page using the kit service.
- LightKitAdminController::getRedirectResponseByRoute &ndash; Creates and returns an HttpRedirectResponse, based on the given arguments.
- LightKitAdminController::checkRight &ndash; Ensures that the current user is connected and has the right provided in the arguments.
- LightKitAdminController::checkMicroPermission &ndash; redirects to the access_denied page.
- LightKitAdminController::error &ndash; Throws an exception.
- LightController::setLight &ndash; Sets the light instance.
- LightController::getLight &ndash; Returns the light application.
- LightController::getContainer &ndash; Returns the service container.
- LightController::getHttpRequest &ndash; Returns the http request bound to the light instance.
- LightController::hasService &ndash; Returns whether the container contains the service which name is given.





Location
=============
Ling\Light_Kit_Admin_TaskScheduler\Controller\Generated\Base\RealGenController<br>
See the source code of [Ling\Light_Kit_Admin_TaskScheduler\Controller\Generated\Base\RealGenController](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/Controller/Generated/Base/RealGenController.php)



SeeAlso
==============
Next class: [LtsTaskScheduleController](https://github.com/lingtalfi/Light_Kit_Admin_TaskScheduler/blob/master/doc/api/Ling/Light_Kit_Admin_TaskScheduler/Controller/Generated/LtsTaskScheduleController.md)<br>
