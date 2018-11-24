# <a name="update-webapp"></a><span data-ttu-id="da3df-101">Update webApp</span><span class="sxs-lookup"><span data-stu-id="da3df-101">Update webApp</span></span>

> <span data-ttu-id="da3df-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="da3df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da3df-103">Обновление свойств объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-103">Update the properties of a [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da3df-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="da3df-104">Prerequisites</span></span>
<span data-ttu-id="da3df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da3df-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da3df-107">Permission type</span></span>|<span data-ttu-id="da3df-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da3df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3df-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da3df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="da3df-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3df-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da3df-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da3df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3df-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3df-112">Not supported.</span></span>|
|<span data-ttu-id="da3df-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da3df-113">Application</span></span>|<span data-ttu-id="da3df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3df-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da3df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="da3df-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da3df-116">Request headers</span></span>
|<span data-ttu-id="da3df-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da3df-117">Header</span></span>|<span data-ttu-id="da3df-118">Значение</span><span class="sxs-lookup"><span data-stu-id="da3df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3df-119">Authorization</span></span>|<span data-ttu-id="da3df-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da3df-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="da3df-121">Accept</span></span>|<span data-ttu-id="da3df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="da3df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3df-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da3df-123">Request body</span></span>
<span data-ttu-id="da3df-124">В тексте запроса добавьте представление объекта [webApp](../resources/intune_apps_webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da3df-124">In the request body, supply a JSON representation for the [webApp](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="da3df-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-125">The following table shows the properties that are required when you create the [webApp](../resources/intune_apps_webapp.md).</span></span>

|<span data-ttu-id="da3df-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="da3df-126">Property</span></span>|<span data-ttu-id="da3df-127">Тип</span><span class="sxs-lookup"><span data-stu-id="da3df-127">Type</span></span>|<span data-ttu-id="da3df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="da3df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da3df-129">id</span><span class="sxs-lookup"><span data-stu-id="da3df-129">id</span></span>|<span data-ttu-id="da3df-130">String</span><span class="sxs-lookup"><span data-stu-id="da3df-130">String</span></span>|<span data-ttu-id="da3df-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="da3df-131">Key of the entity.</span></span> <span data-ttu-id="da3df-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-133">displayName</span><span class="sxs-lookup"><span data-stu-id="da3df-133">displayName</span></span>|<span data-ttu-id="da3df-134">String</span><span class="sxs-lookup"><span data-stu-id="da3df-134">String</span></span>|<span data-ttu-id="da3df-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="da3df-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="da3df-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-137">description</span><span class="sxs-lookup"><span data-stu-id="da3df-137">description</span></span>|<span data-ttu-id="da3df-138">String</span><span class="sxs-lookup"><span data-stu-id="da3df-138">String</span></span>|<span data-ttu-id="da3df-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-139">The description of the app.</span></span> <span data-ttu-id="da3df-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-141">publisher</span><span class="sxs-lookup"><span data-stu-id="da3df-141">publisher</span></span>|<span data-ttu-id="da3df-142">String</span><span class="sxs-lookup"><span data-stu-id="da3df-142">String</span></span>|<span data-ttu-id="da3df-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-143">The publisher of the app.</span></span> <span data-ttu-id="da3df-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="da3df-145">largeIcon</span></span>|[<span data-ttu-id="da3df-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da3df-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="da3df-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="da3df-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="da3df-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da3df-149">createdDateTime</span></span>|<span data-ttu-id="da3df-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3df-150">DateTimeOffset</span></span>|<span data-ttu-id="da3df-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-151">The date and time the app was created.</span></span> <span data-ttu-id="da3df-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da3df-153">lastModifiedDateTime</span></span>|<span data-ttu-id="da3df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3df-154">DateTimeOffset</span></span>|<span data-ttu-id="da3df-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-155">The date and time the app was last modified.</span></span> <span data-ttu-id="da3df-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="da3df-157">isFeatured</span></span>|<span data-ttu-id="da3df-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3df-158">Boolean</span></span>|<span data-ttu-id="da3df-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="da3df-160">privacyInformationUrl</span></span>|<span data-ttu-id="da3df-161">String</span><span class="sxs-lookup"><span data-stu-id="da3df-161">String</span></span>|<span data-ttu-id="da3df-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="da3df-162">The privacy statement Url.</span></span> <span data-ttu-id="da3df-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="da3df-164">informationUrl</span></span>|<span data-ttu-id="da3df-165">String</span><span class="sxs-lookup"><span data-stu-id="da3df-165">String</span></span>|<span data-ttu-id="da3df-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="da3df-166">The more information Url.</span></span> <span data-ttu-id="da3df-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-168">owner</span><span class="sxs-lookup"><span data-stu-id="da3df-168">owner</span></span>|<span data-ttu-id="da3df-169">String</span><span class="sxs-lookup"><span data-stu-id="da3df-169">String</span></span>|<span data-ttu-id="da3df-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-170">The owner of the app.</span></span> <span data-ttu-id="da3df-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-172">developer</span><span class="sxs-lookup"><span data-stu-id="da3df-172">developer</span></span>|<span data-ttu-id="da3df-173">String</span><span class="sxs-lookup"><span data-stu-id="da3df-173">String</span></span>|<span data-ttu-id="da3df-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-174">The developer of the app.</span></span> <span data-ttu-id="da3df-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-176">notes</span><span class="sxs-lookup"><span data-stu-id="da3df-176">notes</span></span>|<span data-ttu-id="da3df-177">String</span><span class="sxs-lookup"><span data-stu-id="da3df-177">String</span></span>|<span data-ttu-id="da3df-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="da3df-178">Notes for the app.</span></span> <span data-ttu-id="da3df-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da3df-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="da3df-180">publishingState</span></span>|[<span data-ttu-id="da3df-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="da3df-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="da3df-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-182">The publishing state for the app.</span></span> <span data-ttu-id="da3df-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="da3df-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="da3df-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="da3df-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="da3df-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="da3df-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="da3df-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="da3df-186">appUrl</span></span>|<span data-ttu-id="da3df-187">String</span><span class="sxs-lookup"><span data-stu-id="da3df-187">String</span></span>|<span data-ttu-id="da3df-188">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="da3df-188">The web app URL.</span></span>|
|<span data-ttu-id="da3df-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="da3df-189">useManagedBrowser</span></span>|<span data-ttu-id="da3df-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3df-190">Boolean</span></span>|<span data-ttu-id="da3df-191">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="da3df-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="da3df-192">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="da3df-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="da3df-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="da3df-193">Response</span></span>
<span data-ttu-id="da3df-194">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune_apps_webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="da3df-194">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3df-195">Пример</span><span class="sxs-lookup"><span data-stu-id="da3df-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="da3df-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="da3df-196">Request</span></span>
<span data-ttu-id="da3df-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da3df-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="da3df-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="da3df-198">Response</span></span>
<span data-ttu-id="da3df-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="da3df-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



