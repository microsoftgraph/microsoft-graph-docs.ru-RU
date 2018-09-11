# <a name="update-managedioslobapp"></a><span data-ttu-id="433c9-101">Обновление managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="433c9-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="433c9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="433c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="433c9-103">Обновление свойств объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-103">Update the properties of a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="433c9-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="433c9-104">Prerequisites</span></span>
<span data-ttu-id="433c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="433c9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="433c9-107">Permission type</span></span>|<span data-ttu-id="433c9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="433c9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="433c9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="433c9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="433c9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="433c9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="433c9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="433c9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="433c9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="433c9-112">Not supported.</span></span>|
|<span data-ttu-id="433c9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="433c9-113">Application</span></span>|<span data-ttu-id="433c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="433c9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="433c9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="433c9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="433c9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="433c9-116">Request headers</span></span>
|<span data-ttu-id="433c9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="433c9-117">Header</span></span>|<span data-ttu-id="433c9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="433c9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="433c9-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="433c9-119">Authorization</span></span>|<span data-ttu-id="433c9-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="433c9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="433c9-121">Принять</span><span class="sxs-lookup"><span data-stu-id="433c9-121">Accept</span></span>|<span data-ttu-id="433c9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="433c9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="433c9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="433c9-123">Request body</span></span>
<span data-ttu-id="433c9-124">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="433c9-124">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="433c9-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-125">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span></span>

|<span data-ttu-id="433c9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="433c9-126">Property</span></span>|<span data-ttu-id="433c9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="433c9-127">Type</span></span>|<span data-ttu-id="433c9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="433c9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="433c9-129">id</span><span class="sxs-lookup"><span data-stu-id="433c9-129">id</span></span>|<span data-ttu-id="433c9-130">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-130">String</span></span>|<span data-ttu-id="433c9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="433c9-131">Key of the entity.</span></span> <span data-ttu-id="433c9-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="433c9-133">displayName</span></span>|<span data-ttu-id="433c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-134">String</span></span>|<span data-ttu-id="433c9-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="433c9-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="433c9-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-137">описание</span><span class="sxs-lookup"><span data-stu-id="433c9-137">description</span></span>|<span data-ttu-id="433c9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-138">String</span></span>|<span data-ttu-id="433c9-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-139">The description of the app.</span></span> <span data-ttu-id="433c9-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-141">publisher</span><span class="sxs-lookup"><span data-stu-id="433c9-141">publisher</span></span>|<span data-ttu-id="433c9-142">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-142">String</span></span>|<span data-ttu-id="433c9-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-143">The publisher of the app.</span></span> <span data-ttu-id="433c9-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="433c9-145">largeIcon</span></span>|[<span data-ttu-id="433c9-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="433c9-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="433c9-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="433c9-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="433c9-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="433c9-149">createdDateTime</span></span>|<span data-ttu-id="433c9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="433c9-150">DateTimeOffset</span></span>|<span data-ttu-id="433c9-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-151">The date and time the app was created.</span></span> <span data-ttu-id="433c9-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="433c9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="433c9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="433c9-154">DateTimeOffset</span></span>|<span data-ttu-id="433c9-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-155">The date and time the app was last modified.</span></span> <span data-ttu-id="433c9-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="433c9-157">isFeatured</span></span>|<span data-ttu-id="433c9-158">Логический</span><span class="sxs-lookup"><span data-stu-id="433c9-158">Boolean</span></span>|<span data-ttu-id="433c9-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="433c9-160">privacyInformationUrl</span></span>|<span data-ttu-id="433c9-161">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-161">String</span></span>|<span data-ttu-id="433c9-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="433c9-162">The privacy statement Url.</span></span> <span data-ttu-id="433c9-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="433c9-164">informationUrl</span></span>|<span data-ttu-id="433c9-165">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-165">String</span></span>|<span data-ttu-id="433c9-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="433c9-166">The more information Url.</span></span> <span data-ttu-id="433c9-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-168">owner</span><span class="sxs-lookup"><span data-stu-id="433c9-168">owner</span></span>|<span data-ttu-id="433c9-169">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-169">String</span></span>|<span data-ttu-id="433c9-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-170">The owner of the app.</span></span> <span data-ttu-id="433c9-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-172">developer</span><span class="sxs-lookup"><span data-stu-id="433c9-172">developer</span></span>|<span data-ttu-id="433c9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-173">String</span></span>|<span data-ttu-id="433c9-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-174">The developer of the app.</span></span> <span data-ttu-id="433c9-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-176">notes</span><span class="sxs-lookup"><span data-stu-id="433c9-176">notes</span></span>|<span data-ttu-id="433c9-177">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-177">String</span></span>|<span data-ttu-id="433c9-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="433c9-178">Notes for the app.</span></span> <span data-ttu-id="433c9-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="433c9-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="433c9-180">publishingState</span></span>|[<span data-ttu-id="433c9-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="433c9-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="433c9-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-182">The publishing state for the app.</span></span> <span data-ttu-id="433c9-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="433c9-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="433c9-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="433c9-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="433c9-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="433c9-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="433c9-186">appAvailability</span></span>|[<span data-ttu-id="433c9-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="433c9-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="433c9-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-188">The Application's availability.</span></span> <span data-ttu-id="433c9-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="433c9-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="433c9-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="433c9-191">version</span><span class="sxs-lookup"><span data-stu-id="433c9-191">version</span></span>|<span data-ttu-id="433c9-192">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-192">String</span></span>|<span data-ttu-id="433c9-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-193">The Application's version.</span></span> <span data-ttu-id="433c9-194">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="433c9-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="433c9-195">committedContentVersion</span></span>|<span data-ttu-id="433c9-196">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-196">String</span></span>|<span data-ttu-id="433c9-197">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="433c9-197">The internal committed content version.</span></span> <span data-ttu-id="433c9-198">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="433c9-199">fileName</span><span class="sxs-lookup"><span data-stu-id="433c9-199">fileName</span></span>|<span data-ttu-id="433c9-200">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-200">String</span></span>|<span data-ttu-id="433c9-201">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="433c9-201">The name of the main Lob application file.</span></span> <span data-ttu-id="433c9-202">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="433c9-203">size</span><span class="sxs-lookup"><span data-stu-id="433c9-203">size</span></span>|<span data-ttu-id="433c9-204">Int64</span><span class="sxs-lookup"><span data-stu-id="433c9-204">Int64</span></span>|<span data-ttu-id="433c9-205">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="433c9-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="433c9-206">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="433c9-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="433c9-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="433c9-207">bundleId</span></span>|<span data-ttu-id="433c9-208">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-208">String</span></span>|<span data-ttu-id="433c9-209">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="433c9-209">The Identity Name.</span></span>|
|<span data-ttu-id="433c9-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="433c9-210">applicableDeviceType</span></span>|[<span data-ttu-id="433c9-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="433c9-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="433c9-212">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="433c9-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="433c9-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="433c9-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="433c9-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="433c9-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="433c9-215">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="433c9-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="433c9-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="433c9-216">expirationDateTime</span></span>|<span data-ttu-id="433c9-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="433c9-217">DateTimeOffset</span></span>|<span data-ttu-id="433c9-218">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="433c9-218">The expiration time.</span></span>|
|<span data-ttu-id="433c9-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="433c9-219">versionNumber</span></span>|<span data-ttu-id="433c9-220">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-220">String</span></span>|<span data-ttu-id="433c9-221">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="433c9-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="433c9-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="433c9-222">buildNumber</span></span>|<span data-ttu-id="433c9-223">Строка</span><span class="sxs-lookup"><span data-stu-id="433c9-223">String</span></span>|<span data-ttu-id="433c9-224">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="433c9-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="433c9-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="433c9-225">Response</span></span>
<span data-ttu-id="433c9-226">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="433c9-226">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="433c9-227">Пример</span><span class="sxs-lookup"><span data-stu-id="433c9-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="433c9-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="433c9-228">Request</span></span>
<span data-ttu-id="433c9-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="433c9-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1276

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="433c9-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="433c9-230">Response</span></span>
<span data-ttu-id="433c9-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="433c9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```








