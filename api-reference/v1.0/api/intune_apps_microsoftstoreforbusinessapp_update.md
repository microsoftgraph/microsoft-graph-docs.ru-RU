# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="8ceb4-101">Обновление microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="8ceb4-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="8ceb4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ceb4-103">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-103">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ceb4-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8ceb4-104">Prerequisites</span></span>
<span data-ttu-id="8ceb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ceb4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ceb4-107">Permission type</span></span>|<span data-ttu-id="8ceb4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ceb4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ceb4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ceb4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ceb4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ceb4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8ceb4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ceb4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ceb4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-112">Not supported.</span></span>|
|<span data-ttu-id="8ceb4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ceb4-113">Application</span></span>|<span data-ttu-id="8ceb4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ceb4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ceb4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8ceb4-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ceb4-116">Request headers</span></span>
|<span data-ttu-id="8ceb4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ceb4-117">Header</span></span>|<span data-ttu-id="8ceb4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8ceb4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ceb4-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ceb4-119">Authorization</span></span>|<span data-ttu-id="8ceb4-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8ceb4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ceb4-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8ceb4-121">Accept</span></span>|<span data-ttu-id="8ceb4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8ceb4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ceb4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ceb4-123">Request body</span></span>
<span data-ttu-id="8ceb4-124">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-124">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="8ceb4-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-125">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="8ceb4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ceb4-126">Property</span></span>|<span data-ttu-id="8ceb4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8ceb4-127">Type</span></span>|<span data-ttu-id="8ceb4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8ceb4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ceb4-129">id</span><span class="sxs-lookup"><span data-stu-id="8ceb4-129">id</span></span>|<span data-ttu-id="8ceb4-130">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-130">String</span></span>|<span data-ttu-id="8ceb4-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-131">Key of the entity.</span></span> <span data-ttu-id="8ceb4-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8ceb4-133">displayName</span></span>|<span data-ttu-id="8ceb4-134">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-134">String</span></span>|<span data-ttu-id="8ceb4-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8ceb4-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-137">description</span><span class="sxs-lookup"><span data-stu-id="8ceb4-137">description</span></span>|<span data-ttu-id="8ceb4-138">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-138">String</span></span>|<span data-ttu-id="8ceb4-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-139">The description of the app.</span></span> <span data-ttu-id="8ceb4-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-141">publisher</span><span class="sxs-lookup"><span data-stu-id="8ceb4-141">publisher</span></span>|<span data-ttu-id="8ceb4-142">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-142">String</span></span>|<span data-ttu-id="8ceb4-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-143">The publisher of the app.</span></span> <span data-ttu-id="8ceb4-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8ceb4-145">largeIcon</span></span>|[<span data-ttu-id="8ceb4-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8ceb4-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="8ceb4-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8ceb4-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceb4-149">createdDateTime</span></span>|<span data-ttu-id="8ceb4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceb4-150">DateTimeOffset</span></span>|<span data-ttu-id="8ceb4-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-151">The date and time the app was created.</span></span> <span data-ttu-id="8ceb4-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceb4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8ceb4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceb4-154">DateTimeOffset</span></span>|<span data-ttu-id="8ceb4-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-155">The date and time the app was last modified.</span></span> <span data-ttu-id="8ceb4-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8ceb4-157">isFeatured</span></span>|<span data-ttu-id="8ceb4-158">Логический</span><span class="sxs-lookup"><span data-stu-id="8ceb4-158">Boolean</span></span>|<span data-ttu-id="8ceb4-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8ceb4-160">privacyInformationUrl</span></span>|<span data-ttu-id="8ceb4-161">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-161">String</span></span>|<span data-ttu-id="8ceb4-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-162">The privacy statement Url.</span></span> <span data-ttu-id="8ceb4-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8ceb4-164">informationUrl</span></span>|<span data-ttu-id="8ceb4-165">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-165">String</span></span>|<span data-ttu-id="8ceb4-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-166">The more information Url.</span></span> <span data-ttu-id="8ceb4-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-168">owner</span><span class="sxs-lookup"><span data-stu-id="8ceb4-168">owner</span></span>|<span data-ttu-id="8ceb4-169">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-169">String</span></span>|<span data-ttu-id="8ceb4-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-170">The owner of the app.</span></span> <span data-ttu-id="8ceb4-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-172">developer</span><span class="sxs-lookup"><span data-stu-id="8ceb4-172">developer</span></span>|<span data-ttu-id="8ceb4-173">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-173">String</span></span>|<span data-ttu-id="8ceb4-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-174">The developer of the app.</span></span> <span data-ttu-id="8ceb4-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-176">notes</span><span class="sxs-lookup"><span data-stu-id="8ceb4-176">notes</span></span>|<span data-ttu-id="8ceb4-177">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-177">String</span></span>|<span data-ttu-id="8ceb4-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-178">Notes for the app.</span></span> <span data-ttu-id="8ceb4-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8ceb4-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="8ceb4-180">publishingState</span></span>|[<span data-ttu-id="8ceb4-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8ceb4-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="8ceb4-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-182">The publishing state for the app.</span></span> <span data-ttu-id="8ceb4-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8ceb4-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ceb4-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="8ceb4-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8ceb4-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8ceb4-186">usedLicenseCount</span></span>|<span data-ttu-id="8ceb4-187">Int32</span><span class="sxs-lookup"><span data-stu-id="8ceb4-187">Int32</span></span>|<span data-ttu-id="8ceb4-188">Количество используемых лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="8ceb4-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8ceb4-189">totalLicenseCount</span></span>|<span data-ttu-id="8ceb4-190">Int32</span><span class="sxs-lookup"><span data-stu-id="8ceb4-190">Int32</span></span>|<span data-ttu-id="8ceb4-191">Общее количество лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="8ceb4-192">productKey</span><span class="sxs-lookup"><span data-stu-id="8ceb4-192">productKey</span></span>|<span data-ttu-id="8ceb4-193">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-193">String</span></span>|<span data-ttu-id="8ceb4-194">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-194">The app product key</span></span>|
|<span data-ttu-id="8ceb4-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="8ceb4-195">licenseType</span></span>|[<span data-ttu-id="8ceb4-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="8ceb4-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="8ceb4-197">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="8ceb4-198">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-198">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="8ceb4-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="8ceb4-199">packageIdentityName</span></span>|<span data-ttu-id="8ceb4-200">String</span><span class="sxs-lookup"><span data-stu-id="8ceb4-200">String</span></span>|<span data-ttu-id="8ceb4-201">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="8ceb4-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ceb4-202">Response</span></span>
<span data-ttu-id="8ceb4-203">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-203">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ceb4-204">Пример</span><span class="sxs-lookup"><span data-stu-id="8ceb4-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ceb4-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ceb4-205">Request</span></span>
<span data-ttu-id="8ceb4-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ceb4-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ceb4-207">Response</span></span>
<span data-ttu-id="8ceb4-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ceb4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








