# <a name="update-managediosstoreapp"></a><span data-ttu-id="cb540-101">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="cb540-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="cb540-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb540-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb540-103">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-103">Update the properties of a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb540-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb540-104">Prerequisites</span></span>
<span data-ttu-id="cb540-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb540-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb540-107">Permission type</span></span>|<span data-ttu-id="cb540-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb540-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb540-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb540-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cb540-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb540-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb540-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb540-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb540-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb540-112">Not supported.</span></span>|
|<span data-ttu-id="cb540-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb540-113">Application</span></span>|<span data-ttu-id="cb540-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb540-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb540-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb540-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cb540-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb540-116">Request headers</span></span>
|<span data-ttu-id="cb540-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb540-117">Header</span></span>|<span data-ttu-id="cb540-118">Значение</span><span class="sxs-lookup"><span data-stu-id="cb540-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb540-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb540-119">Authorization</span></span>|<span data-ttu-id="cb540-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb540-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb540-121">Принять</span><span class="sxs-lookup"><span data-stu-id="cb540-121">Accept</span></span>|<span data-ttu-id="cb540-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cb540-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb540-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb540-123">Request body</span></span>
<span data-ttu-id="cb540-124">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb540-124">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="cb540-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-125">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span></span>

|<span data-ttu-id="cb540-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb540-126">Property</span></span>|<span data-ttu-id="cb540-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cb540-127">Type</span></span>|<span data-ttu-id="cb540-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cb540-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb540-129">id</span><span class="sxs-lookup"><span data-stu-id="cb540-129">id</span></span>|<span data-ttu-id="cb540-130">String</span><span class="sxs-lookup"><span data-stu-id="cb540-130">String</span></span>|<span data-ttu-id="cb540-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb540-131">Key of the entity.</span></span> <span data-ttu-id="cb540-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cb540-133">displayName</span></span>|<span data-ttu-id="cb540-134">String</span><span class="sxs-lookup"><span data-stu-id="cb540-134">String</span></span>|<span data-ttu-id="cb540-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cb540-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb540-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-137">description</span><span class="sxs-lookup"><span data-stu-id="cb540-137">description</span></span>|<span data-ttu-id="cb540-138">String</span><span class="sxs-lookup"><span data-stu-id="cb540-138">String</span></span>|<span data-ttu-id="cb540-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-139">The description of the app.</span></span> <span data-ttu-id="cb540-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-141">издатель</span><span class="sxs-lookup"><span data-stu-id="cb540-141">publisher</span></span>|<span data-ttu-id="cb540-142">String</span><span class="sxs-lookup"><span data-stu-id="cb540-142">String</span></span>|<span data-ttu-id="cb540-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-143">The publisher of the app.</span></span> <span data-ttu-id="cb540-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb540-145">largeIcon</span></span>|[<span data-ttu-id="cb540-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb540-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="cb540-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cb540-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb540-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb540-149">createdDateTime</span></span>|<span data-ttu-id="cb540-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb540-150">DateTimeOffset</span></span>|<span data-ttu-id="cb540-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-151">The date and time the app was created.</span></span> <span data-ttu-id="cb540-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb540-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cb540-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb540-154">DateTimeOffset</span></span>|<span data-ttu-id="cb540-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-155">The date and time the app was last modified.</span></span> <span data-ttu-id="cb540-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb540-157">isFeatured</span></span>|<span data-ttu-id="cb540-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb540-158">Boolean</span></span>|<span data-ttu-id="cb540-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb540-160">privacyInformationUrl</span></span>|<span data-ttu-id="cb540-161">String</span><span class="sxs-lookup"><span data-stu-id="cb540-161">String</span></span>|<span data-ttu-id="cb540-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cb540-162">The privacy statement Url.</span></span> <span data-ttu-id="cb540-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb540-164">informationUrl</span></span>|<span data-ttu-id="cb540-165">String</span><span class="sxs-lookup"><span data-stu-id="cb540-165">String</span></span>|<span data-ttu-id="cb540-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cb540-166">The more information Url.</span></span> <span data-ttu-id="cb540-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-168">owner</span><span class="sxs-lookup"><span data-stu-id="cb540-168">owner</span></span>|<span data-ttu-id="cb540-169">String</span><span class="sxs-lookup"><span data-stu-id="cb540-169">String</span></span>|<span data-ttu-id="cb540-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-170">The owner of the app.</span></span> <span data-ttu-id="cb540-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-172">developer</span><span class="sxs-lookup"><span data-stu-id="cb540-172">developer</span></span>|<span data-ttu-id="cb540-173">String</span><span class="sxs-lookup"><span data-stu-id="cb540-173">String</span></span>|<span data-ttu-id="cb540-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-174">The developer of the app.</span></span> <span data-ttu-id="cb540-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-176">notes</span><span class="sxs-lookup"><span data-stu-id="cb540-176">notes</span></span>|<span data-ttu-id="cb540-177">String</span><span class="sxs-lookup"><span data-stu-id="cb540-177">String</span></span>|<span data-ttu-id="cb540-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="cb540-178">Notes for the app.</span></span> <span data-ttu-id="cb540-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cb540-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb540-180">publishingState</span></span>|[<span data-ttu-id="cb540-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb540-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="cb540-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-182">The publishing state for the app.</span></span> <span data-ttu-id="cb540-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cb540-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb540-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="cb540-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cb540-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb540-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cb540-186">appAvailability</span></span>|[<span data-ttu-id="cb540-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cb540-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="cb540-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-188">The Application's availability.</span></span> <span data-ttu-id="cb540-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb540-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="cb540-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cb540-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cb540-191">version</span><span class="sxs-lookup"><span data-stu-id="cb540-191">version</span></span>|<span data-ttu-id="cb540-192">String</span><span class="sxs-lookup"><span data-stu-id="cb540-192">String</span></span>|<span data-ttu-id="cb540-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-193">The Application's version.</span></span> <span data-ttu-id="cb540-194">Наследуется от [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb540-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="cb540-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="cb540-195">bundleId</span></span>|<span data-ttu-id="cb540-196">String</span><span class="sxs-lookup"><span data-stu-id="cb540-196">String</span></span>|<span data-ttu-id="cb540-197">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="cb540-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="cb540-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cb540-198">appStoreUrl</span></span>|<span data-ttu-id="cb540-199">String</span><span class="sxs-lookup"><span data-stu-id="cb540-199">String</span></span>|<span data-ttu-id="cb540-200">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="cb540-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="cb540-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cb540-201">applicableDeviceType</span></span>|[<span data-ttu-id="cb540-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cb540-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="cb540-203">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cb540-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cb540-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb540-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cb540-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb540-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="cb540-206">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cb540-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cb540-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb540-207">Response</span></span>
<span data-ttu-id="cb540-208">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb540-208">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb540-209">Пример</span><span class="sxs-lookup"><span data-stu-id="cb540-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb540-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb540-210">Request</span></span>
<span data-ttu-id="cb540-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb540-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="cb540-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb540-212">Response</span></span>
<span data-ttu-id="cb540-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb540-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
    "v11_0": true,
    "v12_0": true
  }
}
```



