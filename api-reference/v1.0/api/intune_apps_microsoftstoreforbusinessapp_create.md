# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="6f691-101">Создать microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="6f691-101">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="6f691-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f691-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f691-103">Создание объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-103">Create a new [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f691-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f691-104">Prerequisites</span></span>
<span data-ttu-id="6f691-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f691-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f691-107">Permission type</span></span>|<span data-ttu-id="6f691-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f691-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f691-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f691-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f691-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f691-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f691-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f691-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f691-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f691-112">Not supported.</span></span>|
|<span data-ttu-id="6f691-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f691-113">Application</span></span>|<span data-ttu-id="6f691-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f691-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f691-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f691-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6f691-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f691-116">Request headers</span></span>
|<span data-ttu-id="6f691-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f691-117">Header</span></span>|<span data-ttu-id="6f691-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6f691-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f691-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f691-119">Authorization</span></span>|<span data-ttu-id="6f691-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="6f691-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f691-121">Принять</span><span class="sxs-lookup"><span data-stu-id="6f691-121">Accept</span></span>|<span data-ttu-id="6f691-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6f691-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f691-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f691-123">Request body</span></span>
<span data-ttu-id="6f691-124">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f691-124">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="6f691-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="6f691-125">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="6f691-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f691-126">Property</span></span>|<span data-ttu-id="6f691-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6f691-127">Type</span></span>|<span data-ttu-id="6f691-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6f691-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f691-129">id</span><span class="sxs-lookup"><span data-stu-id="6f691-129">id</span></span>|<span data-ttu-id="6f691-130">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-130">String</span></span>|<span data-ttu-id="6f691-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f691-131">Key of the entity.</span></span> <span data-ttu-id="6f691-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6f691-133">displayName</span></span>|<span data-ttu-id="6f691-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-134">String</span></span>|<span data-ttu-id="6f691-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6f691-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6f691-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-137">description</span><span class="sxs-lookup"><span data-stu-id="6f691-137">description</span></span>|<span data-ttu-id="6f691-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-138">String</span></span>|<span data-ttu-id="6f691-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-139">The description of the app.</span></span> <span data-ttu-id="6f691-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-141">publisher</span><span class="sxs-lookup"><span data-stu-id="6f691-141">publisher</span></span>|<span data-ttu-id="6f691-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-142">String</span></span>|<span data-ttu-id="6f691-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-143">The publisher of the app.</span></span> <span data-ttu-id="6f691-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6f691-145">largeIcon</span></span>|[<span data-ttu-id="6f691-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6f691-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="6f691-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6f691-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6f691-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f691-149">createdDateTime</span></span>|<span data-ttu-id="6f691-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f691-150">DateTimeOffset</span></span>|<span data-ttu-id="6f691-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-151">The date and time the app was created.</span></span> <span data-ttu-id="6f691-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f691-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6f691-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f691-154">DateTimeOffset</span></span>|<span data-ttu-id="6f691-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-155">The date and time the app was last modified.</span></span> <span data-ttu-id="6f691-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6f691-157">isFeatured</span></span>|<span data-ttu-id="6f691-158">Логический</span><span class="sxs-lookup"><span data-stu-id="6f691-158">Boolean</span></span>|<span data-ttu-id="6f691-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6f691-160">privacyInformationUrl</span></span>|<span data-ttu-id="6f691-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-161">String</span></span>|<span data-ttu-id="6f691-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6f691-162">The privacy statement Url.</span></span> <span data-ttu-id="6f691-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6f691-164">informationUrl</span></span>|<span data-ttu-id="6f691-165">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-165">String</span></span>|<span data-ttu-id="6f691-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6f691-166">The more information Url.</span></span> <span data-ttu-id="6f691-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-168">owner</span><span class="sxs-lookup"><span data-stu-id="6f691-168">owner</span></span>|<span data-ttu-id="6f691-169">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-169">String</span></span>|<span data-ttu-id="6f691-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-170">The owner of the app.</span></span> <span data-ttu-id="6f691-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-172">developer</span><span class="sxs-lookup"><span data-stu-id="6f691-172">developer</span></span>|<span data-ttu-id="6f691-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-173">String</span></span>|<span data-ttu-id="6f691-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-174">The developer of the app.</span></span> <span data-ttu-id="6f691-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-176">notes</span><span class="sxs-lookup"><span data-stu-id="6f691-176">notes</span></span>|<span data-ttu-id="6f691-177">Строка</span><span class="sxs-lookup"><span data-stu-id="6f691-177">String</span></span>|<span data-ttu-id="6f691-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="6f691-178">Notes for the app.</span></span> <span data-ttu-id="6f691-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f691-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6f691-180">publishingState</span></span>|[<span data-ttu-id="6f691-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6f691-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="6f691-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-182">The publishing state for the app.</span></span> <span data-ttu-id="6f691-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6f691-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6f691-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f691-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="6f691-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6f691-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6f691-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6f691-186">usedLicenseCount</span></span>|<span data-ttu-id="6f691-187">Int32</span><span class="sxs-lookup"><span data-stu-id="6f691-187">Int32</span></span>|<span data-ttu-id="6f691-188">Количество используемых лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6f691-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="6f691-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6f691-189">totalLicenseCount</span></span>|<span data-ttu-id="6f691-190">Int32</span><span class="sxs-lookup"><span data-stu-id="6f691-190">Int32</span></span>|<span data-ttu-id="6f691-191">Общее количество лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6f691-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="6f691-192">productKey</span><span class="sxs-lookup"><span data-stu-id="6f691-192">productKey</span></span>|<span data-ttu-id="6f691-193">String</span><span class="sxs-lookup"><span data-stu-id="6f691-193">String</span></span>|<span data-ttu-id="6f691-194">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-194">The app product key</span></span>|
|<span data-ttu-id="6f691-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="6f691-195">licenseType</span></span>|[<span data-ttu-id="6f691-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="6f691-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="6f691-197">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="6f691-198">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="6f691-198">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="6f691-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="6f691-199">packageIdentityName</span></span>|<span data-ttu-id="6f691-200">String</span><span class="sxs-lookup"><span data-stu-id="6f691-200">String</span></span>|<span data-ttu-id="6f691-201">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="6f691-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="6f691-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f691-202">Response</span></span>
<span data-ttu-id="6f691-203">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6f691-203">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f691-204">Пример</span><span class="sxs-lookup"><span data-stu-id="6f691-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f691-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f691-205">Request</span></span>
<span data-ttu-id="6f691-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f691-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 833

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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

### <a name="response"></a><span data-ttu-id="6f691-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f691-207">Response</span></span>
<span data-ttu-id="6f691-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f691-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








