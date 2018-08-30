# <a name="create-iosstoreapp"></a><span data-ttu-id="a2954-101">Создание iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="a2954-101">Create iosStoreApp</span></span>

> <span data-ttu-id="a2954-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2954-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2954-103">Создание объекта [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-103">Create a new [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2954-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a2954-104">Prerequisites</span></span>
<span data-ttu-id="a2954-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2954-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2954-107">Permission type</span></span>|<span data-ttu-id="a2954-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2954-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2954-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2954-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2954-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2954-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2954-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2954-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2954-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2954-112">Not supported.</span></span>|
|<span data-ttu-id="a2954-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2954-113">Application</span></span>|<span data-ttu-id="a2954-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2954-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2954-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2954-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a2954-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2954-116">Request headers</span></span>
|<span data-ttu-id="a2954-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2954-117">Header</span></span>|<span data-ttu-id="a2954-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a2954-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2954-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2954-119">Authorization</span></span>|<span data-ttu-id="a2954-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a2954-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2954-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a2954-121">Accept</span></span>|<span data-ttu-id="a2954-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a2954-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2954-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2954-123">Request body</span></span>
<span data-ttu-id="a2954-124">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2954-124">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="a2954-125">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a2954-125">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="a2954-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2954-126">Property</span></span>|<span data-ttu-id="a2954-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a2954-127">Type</span></span>|<span data-ttu-id="a2954-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a2954-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2954-129">id</span><span class="sxs-lookup"><span data-stu-id="a2954-129">id</span></span>|<span data-ttu-id="a2954-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-130">String</span></span>|<span data-ttu-id="a2954-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2954-131">Key of the entity.</span></span> <span data-ttu-id="a2954-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a2954-133">displayName</span></span>|<span data-ttu-id="a2954-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-134">String</span></span>|<span data-ttu-id="a2954-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a2954-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a2954-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-137">description</span><span class="sxs-lookup"><span data-stu-id="a2954-137">description</span></span>|<span data-ttu-id="a2954-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-138">String</span></span>|<span data-ttu-id="a2954-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-139">The description of the app.</span></span> <span data-ttu-id="a2954-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-141">publisher</span><span class="sxs-lookup"><span data-stu-id="a2954-141">publisher</span></span>|<span data-ttu-id="a2954-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-142">String</span></span>|<span data-ttu-id="a2954-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-143">The publisher of the app.</span></span> <span data-ttu-id="a2954-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a2954-145">largeIcon</span></span>|[<span data-ttu-id="a2954-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a2954-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="a2954-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a2954-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a2954-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2954-149">createdDateTime</span></span>|<span data-ttu-id="a2954-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2954-150">DateTimeOffset</span></span>|<span data-ttu-id="a2954-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-151">The date and time the app was created.</span></span> <span data-ttu-id="a2954-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2954-153">lastModifiedDateTime</span></span>|<span data-ttu-id="a2954-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2954-154">DateTimeOffset</span></span>|<span data-ttu-id="a2954-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-155">The date and time the app was last modified.</span></span> <span data-ttu-id="a2954-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a2954-157">isFeatured</span></span>|<span data-ttu-id="a2954-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="a2954-158">Boolean</span></span>|<span data-ttu-id="a2954-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a2954-160">privacyInformationUrl</span></span>|<span data-ttu-id="a2954-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-161">String</span></span>|<span data-ttu-id="a2954-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a2954-162">The privacy statement Url.</span></span> <span data-ttu-id="a2954-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a2954-164">informationUrl</span></span>|<span data-ttu-id="a2954-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-165">String</span></span>|<span data-ttu-id="a2954-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a2954-166">The more information Url.</span></span> <span data-ttu-id="a2954-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-168">owner</span><span class="sxs-lookup"><span data-stu-id="a2954-168">owner</span></span>|<span data-ttu-id="a2954-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-169">String</span></span>|<span data-ttu-id="a2954-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-170">The owner of the app.</span></span> <span data-ttu-id="a2954-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-172">developer</span><span class="sxs-lookup"><span data-stu-id="a2954-172">developer</span></span>|<span data-ttu-id="a2954-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-173">String</span></span>|<span data-ttu-id="a2954-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-174">The developer of the app.</span></span> <span data-ttu-id="a2954-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-176">notes</span><span class="sxs-lookup"><span data-stu-id="a2954-176">notes</span></span>|<span data-ttu-id="a2954-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-177">String</span></span>|<span data-ttu-id="a2954-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a2954-178">Notes for the app.</span></span> <span data-ttu-id="a2954-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a2954-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="a2954-180">publishingState</span></span>|[<span data-ttu-id="a2954-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a2954-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="a2954-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a2954-182">The publishing state for the app.</span></span> <span data-ttu-id="a2954-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a2954-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a2954-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2954-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="a2954-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a2954-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="a2954-186">bundleId</span><span class="sxs-lookup"><span data-stu-id="a2954-186">bundleId</span></span>|<span data-ttu-id="a2954-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-187">String</span></span>|<span data-ttu-id="a2954-188">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a2954-188">The Identity Name.</span></span>|
|<span data-ttu-id="a2954-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a2954-189">appStoreUrl</span></span>|<span data-ttu-id="a2954-190">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2954-190">String</span></span>|<span data-ttu-id="a2954-191">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="a2954-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="a2954-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a2954-192">applicableDeviceType</span></span>|[<span data-ttu-id="a2954-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a2954-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="a2954-194">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a2954-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="a2954-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a2954-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a2954-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a2954-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="a2954-197">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a2954-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a2954-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2954-198">Response</span></span>
<span data-ttu-id="a2954-199">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune_apps_iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2954-199">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2954-200">Пример</span><span class="sxs-lookup"><span data-stu-id="a2954-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2954-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2954-201">Request</span></span>
<span data-ttu-id="a2954-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2954-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a2954-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2954-203">Response</span></span>
<span data-ttu-id="a2954-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2954-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1158

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
    "v11_0": true
  }
}
```



