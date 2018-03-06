# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="d055e-101">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="d055e-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="d055e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d055e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d055e-103">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-103">Update the properties of a [calendar](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d055e-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d055e-104">Prerequisites</span></span>
<span data-ttu-id="d055e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d055e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d055e-107">Permission type</span></span>|<span data-ttu-id="d055e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d055e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d055e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d055e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d055e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d055e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d055e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d055e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d055e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d055e-112">Not supported.</span></span>|
|<span data-ttu-id="d055e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d055e-113">Application</span></span>|<span data-ttu-id="d055e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d055e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d055e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d055e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d055e-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d055e-116">Request headers</span></span>
|<span data-ttu-id="d055e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d055e-117">Header</span></span>|<span data-ttu-id="d055e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d055e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d055e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d055e-119">Authorization</span></span>|<span data-ttu-id="d055e-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d055e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d055e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d055e-121">Accept</span></span>|<span data-ttu-id="d055e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d055e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d055e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d055e-123">Request body</span></span>
<span data-ttu-id="d055e-124">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d055e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="d055e-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d055e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d055e-126">Property</span></span>|<span data-ttu-id="d055e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d055e-127">Type</span></span>|<span data-ttu-id="d055e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d055e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d055e-129">id</span><span class="sxs-lookup"><span data-stu-id="d055e-129">id</span></span>|<span data-ttu-id="d055e-130">String</span><span class="sxs-lookup"><span data-stu-id="d055e-130">String</span></span>|<span data-ttu-id="d055e-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d055e-131">Key of the setting.</span></span> <span data-ttu-id="d055e-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d055e-133">displayName</span></span>|<span data-ttu-id="d055e-134">String</span><span class="sxs-lookup"><span data-stu-id="d055e-134">String</span></span>|<span data-ttu-id="d055e-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d055e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d055e-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-137">description</span><span class="sxs-lookup"><span data-stu-id="d055e-137">description</span></span>|<span data-ttu-id="d055e-138">String</span><span class="sxs-lookup"><span data-stu-id="d055e-138">String</span></span>|<span data-ttu-id="d055e-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-139">The description of the app.</span></span> <span data-ttu-id="d055e-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d055e-141">Publisher</span></span>|<span data-ttu-id="d055e-142">String</span><span class="sxs-lookup"><span data-stu-id="d055e-142">String</span></span>|<span data-ttu-id="d055e-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-143">The name of the app.</span></span> <span data-ttu-id="d055e-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d055e-145">largeIcon</span></span>|[<span data-ttu-id="d055e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d055e-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="d055e-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d055e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d055e-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d055e-149">createdDateTime</span></span>|<span data-ttu-id="d055e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d055e-150">DateTimeOffset</span></span>|<span data-ttu-id="d055e-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-151">The date and time the group was created.</span></span> <span data-ttu-id="d055e-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d055e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d055e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d055e-154">DateTimeOffset</span></span>|<span data-ttu-id="d055e-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="d055e-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d055e-157">isFeatured</span></span>|<span data-ttu-id="d055e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d055e-158">Boolean</span></span>|<span data-ttu-id="d055e-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d055e-160">privacyInformationUrl</span></span>|<span data-ttu-id="d055e-161">String</span><span class="sxs-lookup"><span data-stu-id="d055e-161">String</span></span>|<span data-ttu-id="d055e-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d055e-162">The privacy statement Url.</span></span> <span data-ttu-id="d055e-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d055e-164">informationUrl</span></span>|<span data-ttu-id="d055e-165">String</span><span class="sxs-lookup"><span data-stu-id="d055e-165">String</span></span>|<span data-ttu-id="d055e-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d055e-166">The more information Url.</span></span> <span data-ttu-id="d055e-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-168">owner</span><span class="sxs-lookup"><span data-stu-id="d055e-168">owner</span></span>|<span data-ttu-id="d055e-169">String</span><span class="sxs-lookup"><span data-stu-id="d055e-169">String</span></span>|<span data-ttu-id="d055e-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-170">The owner of the app.</span></span> <span data-ttu-id="d055e-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-172">developer</span><span class="sxs-lookup"><span data-stu-id="d055e-172">developer</span></span>|<span data-ttu-id="d055e-173">String</span><span class="sxs-lookup"><span data-stu-id="d055e-173">String</span></span>|<span data-ttu-id="d055e-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-174">The name of the app.</span></span> <span data-ttu-id="d055e-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-176">notes</span><span class="sxs-lookup"><span data-stu-id="d055e-176">Notes</span></span>|<span data-ttu-id="d055e-177">String</span><span class="sxs-lookup"><span data-stu-id="d055e-177">String</span></span>|<span data-ttu-id="d055e-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-178">Notes for the app.</span></span> <span data-ttu-id="d055e-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d055e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d055e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d055e-180">publishingState</span></span>|<span data-ttu-id="d055e-181">String</span><span class="sxs-lookup"><span data-stu-id="d055e-181">String</span></span>|<span data-ttu-id="d055e-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-182">The publishing state for the app.</span></span> <span data-ttu-id="d055e-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d055e-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d055e-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d055e-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d055e-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d055e-185">usedLicenseCount</span></span>|<span data-ttu-id="d055e-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d055e-186">Int32</span></span>|<span data-ttu-id="d055e-187">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d055e-187">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="d055e-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d055e-188">totalLicenseCount</span></span>|<span data-ttu-id="d055e-189">Int32</span><span class="sxs-lookup"><span data-stu-id="d055e-189">Int32</span></span>|<span data-ttu-id="d055e-190">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d055e-190">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="d055e-191">productKey</span><span class="sxs-lookup"><span data-stu-id="d055e-191">productKey</span></span>|<span data-ttu-id="d055e-192">String</span><span class="sxs-lookup"><span data-stu-id="d055e-192">String</span></span>|<span data-ttu-id="d055e-193">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="d055e-193">The app product key</span></span>|
|<span data-ttu-id="d055e-194">licenseType</span><span class="sxs-lookup"><span data-stu-id="d055e-194">licenseType</span></span>|<span data-ttu-id="d055e-195">String</span><span class="sxs-lookup"><span data-stu-id="d055e-195">String</span></span>|<span data-ttu-id="d055e-196">Тип лицензии для приложения. Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="d055e-196">The app license type Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="d055e-197">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="d055e-197">packageIdentityName</span></span>|<span data-ttu-id="d055e-198">String</span><span class="sxs-lookup"><span data-stu-id="d055e-198">String</span></span>|<span data-ttu-id="d055e-199">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="d055e-199">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="d055e-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="d055e-200">Response</span></span>
<span data-ttu-id="d055e-201">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d055e-201">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d055e-202">Пример</span><span class="sxs-lookup"><span data-stu-id="d055e-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="d055e-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="d055e-203">Request</span></span>
<span data-ttu-id="d055e-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d055e-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 766

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="d055e-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="d055e-205">Response</span></span>
<span data-ttu-id="d055e-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d055e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



