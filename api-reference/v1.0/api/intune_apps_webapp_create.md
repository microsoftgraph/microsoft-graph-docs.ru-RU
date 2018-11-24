# <a name="create-webapp"></a><span data-ttu-id="85ba8-101">Create webApp</span><span class="sxs-lookup"><span data-stu-id="85ba8-101">Create webApp</span></span>

> <span data-ttu-id="85ba8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85ba8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85ba8-103">Создание объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-103">Create a new [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85ba8-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="85ba8-104">Prerequisites</span></span>
<span data-ttu-id="85ba8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85ba8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85ba8-107">Permission type</span></span>|<span data-ttu-id="85ba8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85ba8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85ba8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85ba8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="85ba8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ba8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85ba8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85ba8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85ba8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ba8-112">Not supported.</span></span>|
|<span data-ttu-id="85ba8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85ba8-113">Application</span></span>|<span data-ttu-id="85ba8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ba8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85ba8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85ba8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="85ba8-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85ba8-116">Request headers</span></span>
|<span data-ttu-id="85ba8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85ba8-117">Header</span></span>|<span data-ttu-id="85ba8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="85ba8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85ba8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="85ba8-119">Authorization</span></span>|<span data-ttu-id="85ba8-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85ba8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85ba8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="85ba8-121">Accept</span></span>|<span data-ttu-id="85ba8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="85ba8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85ba8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85ba8-123">Request body</span></span>
<span data-ttu-id="85ba8-124">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85ba8-124">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="85ba8-125">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="85ba8-125">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="85ba8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="85ba8-126">Property</span></span>|<span data-ttu-id="85ba8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="85ba8-127">Type</span></span>|<span data-ttu-id="85ba8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="85ba8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85ba8-129">id</span><span class="sxs-lookup"><span data-stu-id="85ba8-129">id</span></span>|<span data-ttu-id="85ba8-130">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-130">String</span></span>|<span data-ttu-id="85ba8-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85ba8-131">Key of the entity.</span></span> <span data-ttu-id="85ba8-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="85ba8-133">displayName</span></span>|<span data-ttu-id="85ba8-134">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-134">String</span></span>|<span data-ttu-id="85ba8-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="85ba8-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85ba8-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-137">description</span><span class="sxs-lookup"><span data-stu-id="85ba8-137">description</span></span>|<span data-ttu-id="85ba8-138">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-138">String</span></span>|<span data-ttu-id="85ba8-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-139">The description of the app.</span></span> <span data-ttu-id="85ba8-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-141">publisher</span><span class="sxs-lookup"><span data-stu-id="85ba8-141">publisher</span></span>|<span data-ttu-id="85ba8-142">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-142">String</span></span>|<span data-ttu-id="85ba8-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-143">The publisher of the app.</span></span> <span data-ttu-id="85ba8-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85ba8-145">largeIcon</span></span>|[<span data-ttu-id="85ba8-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85ba8-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="85ba8-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="85ba8-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85ba8-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85ba8-149">createdDateTime</span></span>|<span data-ttu-id="85ba8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85ba8-150">DateTimeOffset</span></span>|<span data-ttu-id="85ba8-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-151">The date and time the app was created.</span></span> <span data-ttu-id="85ba8-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85ba8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="85ba8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85ba8-154">DateTimeOffset</span></span>|<span data-ttu-id="85ba8-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-155">The date and time the app was last modified.</span></span> <span data-ttu-id="85ba8-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85ba8-157">isFeatured</span></span>|<span data-ttu-id="85ba8-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="85ba8-158">Boolean</span></span>|<span data-ttu-id="85ba8-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85ba8-160">privacyInformationUrl</span></span>|<span data-ttu-id="85ba8-161">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-161">String</span></span>|<span data-ttu-id="85ba8-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="85ba8-162">The privacy statement Url.</span></span> <span data-ttu-id="85ba8-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85ba8-164">informationUrl</span></span>|<span data-ttu-id="85ba8-165">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-165">String</span></span>|<span data-ttu-id="85ba8-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="85ba8-166">The more information Url.</span></span> <span data-ttu-id="85ba8-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-168">owner</span><span class="sxs-lookup"><span data-stu-id="85ba8-168">owner</span></span>|<span data-ttu-id="85ba8-169">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-169">String</span></span>|<span data-ttu-id="85ba8-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-170">The owner of the app.</span></span> <span data-ttu-id="85ba8-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-172">developer</span><span class="sxs-lookup"><span data-stu-id="85ba8-172">developer</span></span>|<span data-ttu-id="85ba8-173">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-173">String</span></span>|<span data-ttu-id="85ba8-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-174">The developer of the app.</span></span> <span data-ttu-id="85ba8-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-176">notes</span><span class="sxs-lookup"><span data-stu-id="85ba8-176">notes</span></span>|<span data-ttu-id="85ba8-177">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-177">String</span></span>|<span data-ttu-id="85ba8-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="85ba8-178">Notes for the app.</span></span> <span data-ttu-id="85ba8-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="85ba8-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="85ba8-180">publishingState</span></span>|[<span data-ttu-id="85ba8-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="85ba8-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="85ba8-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-182">The publishing state for the app.</span></span> <span data-ttu-id="85ba8-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="85ba8-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85ba8-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85ba8-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="85ba8-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="85ba8-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="85ba8-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="85ba8-186">appUrl</span></span>|<span data-ttu-id="85ba8-187">String</span><span class="sxs-lookup"><span data-stu-id="85ba8-187">String</span></span>|<span data-ttu-id="85ba8-188">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="85ba8-188">The web app URL.</span></span>|
|<span data-ttu-id="85ba8-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="85ba8-189">useManagedBrowser</span></span>|<span data-ttu-id="85ba8-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="85ba8-190">Boolean</span></span>|<span data-ttu-id="85ba8-191">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="85ba8-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="85ba8-192">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="85ba8-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="85ba8-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="85ba8-193">Response</span></span>
<span data-ttu-id="85ba8-194">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune_apps_webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85ba8-194">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85ba8-195">Пример</span><span class="sxs-lookup"><span data-stu-id="85ba8-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="85ba8-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="85ba8-196">Request</span></span>
<span data-ttu-id="85ba8-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85ba8-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="85ba8-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="85ba8-198">Response</span></span>
<span data-ttu-id="85ba8-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="85ba8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



