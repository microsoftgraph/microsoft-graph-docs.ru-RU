# <a name="create-iosstoreapp"></a><span data-ttu-id="5bccb-101">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="5bccb-101">Create iosStoreApp</span></span>

> <span data-ttu-id="5bccb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5bccb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bccb-103">Создание объекта [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-103">Create a new [plannerBucket](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bccb-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5bccb-104">Prerequisites</span></span>
<span data-ttu-id="5bccb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5bccb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bccb-107">Permission type</span></span>|<span data-ttu-id="5bccb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bccb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bccb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bccb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5bccb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bccb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bccb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bccb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bccb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bccb-112">Not supported.</span></span>|
|<span data-ttu-id="5bccb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bccb-113">Application</span></span>|<span data-ttu-id="5bccb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bccb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bccb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bccb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5bccb-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5bccb-116">Request headers</span></span>
|<span data-ttu-id="5bccb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bccb-117">Header</span></span>|<span data-ttu-id="5bccb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5bccb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bccb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bccb-119">Authorization</span></span>|<span data-ttu-id="5bccb-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bccb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5bccb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5bccb-121">Accept</span></span>|<span data-ttu-id="5bccb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5bccb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bccb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bccb-123">Request body</span></span>
<span data-ttu-id="5bccb-124">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bccb-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5bccb-125">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="5bccb-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5bccb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bccb-126">Property</span></span>|<span data-ttu-id="5bccb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5bccb-127">Type</span></span>|<span data-ttu-id="5bccb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5bccb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bccb-129">id</span><span class="sxs-lookup"><span data-stu-id="5bccb-129">id</span></span>|<span data-ttu-id="5bccb-130">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-130">String</span></span>|<span data-ttu-id="5bccb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5bccb-131">Key of the setting.</span></span> <span data-ttu-id="5bccb-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5bccb-133">displayName</span></span>|<span data-ttu-id="5bccb-134">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-134">String</span></span>|<span data-ttu-id="5bccb-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5bccb-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5bccb-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-137">description</span><span class="sxs-lookup"><span data-stu-id="5bccb-137">description</span></span>|<span data-ttu-id="5bccb-138">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-138">String</span></span>|<span data-ttu-id="5bccb-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-139">The description of the app.</span></span> <span data-ttu-id="5bccb-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-141">publisher</span><span class="sxs-lookup"><span data-stu-id="5bccb-141">Publisher</span></span>|<span data-ttu-id="5bccb-142">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-142">String</span></span>|<span data-ttu-id="5bccb-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-143">The name of the app.</span></span> <span data-ttu-id="5bccb-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5bccb-145">largeIcon</span></span>|[<span data-ttu-id="5bccb-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5bccb-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="5bccb-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5bccb-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5bccb-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bccb-149">createdDateTime</span></span>|<span data-ttu-id="5bccb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bccb-150">DateTimeOffset</span></span>|<span data-ttu-id="5bccb-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-151">The date and time the group was created.</span></span> <span data-ttu-id="5bccb-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bccb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5bccb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bccb-154">DateTimeOffset</span></span>|<span data-ttu-id="5bccb-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="5bccb-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5bccb-157">isFeatured</span></span>|<span data-ttu-id="5bccb-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bccb-158">Boolean</span></span>|<span data-ttu-id="5bccb-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5bccb-160">privacyInformationUrl</span></span>|<span data-ttu-id="5bccb-161">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-161">String</span></span>|<span data-ttu-id="5bccb-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5bccb-162">The privacy statement Url.</span></span> <span data-ttu-id="5bccb-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5bccb-164">informationUrl</span></span>|<span data-ttu-id="5bccb-165">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-165">String</span></span>|<span data-ttu-id="5bccb-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5bccb-166">The more information Url.</span></span> <span data-ttu-id="5bccb-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-168">owner</span><span class="sxs-lookup"><span data-stu-id="5bccb-168">owner</span></span>|<span data-ttu-id="5bccb-169">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-169">String</span></span>|<span data-ttu-id="5bccb-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-170">The owner of the app.</span></span> <span data-ttu-id="5bccb-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-172">developer</span><span class="sxs-lookup"><span data-stu-id="5bccb-172">developer</span></span>|<span data-ttu-id="5bccb-173">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-173">String</span></span>|<span data-ttu-id="5bccb-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-174">The name of the app.</span></span> <span data-ttu-id="5bccb-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-176">notes</span><span class="sxs-lookup"><span data-stu-id="5bccb-176">Notes</span></span>|<span data-ttu-id="5bccb-177">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-177">String</span></span>|<span data-ttu-id="5bccb-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-178">Notes for the app.</span></span> <span data-ttu-id="5bccb-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bccb-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bccb-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="5bccb-180">publishingState</span></span>|<span data-ttu-id="5bccb-181">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-181">String</span></span>|<span data-ttu-id="5bccb-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-182">The publishing state for the app.</span></span> <span data-ttu-id="5bccb-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5bccb-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5bccb-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5bccb-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5bccb-185">bundleId</span><span class="sxs-lookup"><span data-stu-id="5bccb-185">bundleId</span></span>|<span data-ttu-id="5bccb-186">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-186">String</span></span>|<span data-ttu-id="5bccb-187">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5bccb-187">The Identity Name.</span></span>|
|<span data-ttu-id="5bccb-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5bccb-188">appStoreUrl</span></span>|<span data-ttu-id="5bccb-189">String</span><span class="sxs-lookup"><span data-stu-id="5bccb-189">String</span></span>|<span data-ttu-id="5bccb-190">URL-адрес магазина приложений Apple</span><span class="sxs-lookup"><span data-stu-id="5bccb-190">The Apple App Store URL</span></span>|
|<span data-ttu-id="5bccb-191">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5bccb-191">applicableDeviceType</span></span>|[<span data-ttu-id="5bccb-192">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5bccb-192">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="5bccb-193">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="5bccb-193">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5bccb-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5bccb-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5bccb-195">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5bccb-195">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="5bccb-196">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5bccb-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5bccb-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="5bccb-197">Response</span></span>
<span data-ttu-id="5bccb-198">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune_apps_iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5bccb-198">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bccb-199">Пример</span><span class="sxs-lookup"><span data-stu-id="5bccb-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bccb-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bccb-200">Request</span></span>
<span data-ttu-id="5bccb-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bccb-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bccb-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="5bccb-202">Response</span></span>
<span data-ttu-id="5bccb-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5bccb-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



