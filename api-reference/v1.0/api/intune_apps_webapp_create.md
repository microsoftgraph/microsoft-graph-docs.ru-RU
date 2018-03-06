# <a name="create-webapp"></a><span data-ttu-id="cd9ed-101">Create webApp</span><span class="sxs-lookup"><span data-stu-id="cd9ed-101">Create webApp</span></span>

> <span data-ttu-id="cd9ed-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd9ed-103">Создание объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-103">Create a new [plannerBucket](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd9ed-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9ed-104">Prerequisites</span></span>
<span data-ttu-id="cd9ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd9ed-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9ed-107">Permission type</span></span>|<span data-ttu-id="cd9ed-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd9ed-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9ed-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd9ed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9ed-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9ed-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9ed-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd9ed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9ed-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-112">Not supported.</span></span>|
|<span data-ttu-id="cd9ed-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd9ed-113">Application</span></span>|<span data-ttu-id="cd9ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9ed-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd9ed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cd9ed-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd9ed-116">Request headers</span></span>
|<span data-ttu-id="cd9ed-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd9ed-117">Header</span></span>|<span data-ttu-id="cd9ed-118">Значение</span><span class="sxs-lookup"><span data-stu-id="cd9ed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9ed-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9ed-119">Authorization</span></span>|<span data-ttu-id="cd9ed-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cd9ed-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cd9ed-121">Accept</span></span>|<span data-ttu-id="cd9ed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9ed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9ed-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd9ed-123">Request body</span></span>
<span data-ttu-id="cd9ed-124">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="cd9ed-125">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="cd9ed-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd9ed-126">Property</span></span>|<span data-ttu-id="cd9ed-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cd9ed-127">Type</span></span>|<span data-ttu-id="cd9ed-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cd9ed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9ed-129">id</span><span class="sxs-lookup"><span data-stu-id="cd9ed-129">id</span></span>|<span data-ttu-id="cd9ed-130">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-130">String</span></span>|<span data-ttu-id="cd9ed-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-131">Key of the setting.</span></span> <span data-ttu-id="cd9ed-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cd9ed-133">displayName</span></span>|<span data-ttu-id="cd9ed-134">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-134">String</span></span>|<span data-ttu-id="cd9ed-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cd9ed-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-137">description</span><span class="sxs-lookup"><span data-stu-id="cd9ed-137">description</span></span>|<span data-ttu-id="cd9ed-138">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-138">String</span></span>|<span data-ttu-id="cd9ed-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-139">The description of the app.</span></span> <span data-ttu-id="cd9ed-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-141">publisher</span><span class="sxs-lookup"><span data-stu-id="cd9ed-141">Publisher</span></span>|<span data-ttu-id="cd9ed-142">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-142">String</span></span>|<span data-ttu-id="cd9ed-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-143">The name of the app.</span></span> <span data-ttu-id="cd9ed-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cd9ed-145">largeIcon</span></span>|[<span data-ttu-id="cd9ed-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd9ed-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="cd9ed-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cd9ed-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd9ed-149">createdDateTime</span></span>|<span data-ttu-id="cd9ed-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9ed-150">DateTimeOffset</span></span>|<span data-ttu-id="cd9ed-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-151">The date and time the group was created.</span></span> <span data-ttu-id="cd9ed-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd9ed-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cd9ed-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9ed-154">DateTimeOffset</span></span>|<span data-ttu-id="cd9ed-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="cd9ed-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cd9ed-157">isFeatured</span></span>|<span data-ttu-id="cd9ed-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd9ed-158">Boolean</span></span>|<span data-ttu-id="cd9ed-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd9ed-160">privacyInformationUrl</span></span>|<span data-ttu-id="cd9ed-161">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-161">String</span></span>|<span data-ttu-id="cd9ed-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-162">The privacy statement Url.</span></span> <span data-ttu-id="cd9ed-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd9ed-164">informationUrl</span></span>|<span data-ttu-id="cd9ed-165">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-165">String</span></span>|<span data-ttu-id="cd9ed-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-166">The more information Url.</span></span> <span data-ttu-id="cd9ed-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-168">owner</span><span class="sxs-lookup"><span data-stu-id="cd9ed-168">owner</span></span>|<span data-ttu-id="cd9ed-169">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-169">String</span></span>|<span data-ttu-id="cd9ed-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-170">The owner of the app.</span></span> <span data-ttu-id="cd9ed-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-172">developer</span><span class="sxs-lookup"><span data-stu-id="cd9ed-172">developer</span></span>|<span data-ttu-id="cd9ed-173">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-173">String</span></span>|<span data-ttu-id="cd9ed-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-174">The name of the app.</span></span> <span data-ttu-id="cd9ed-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-176">notes</span><span class="sxs-lookup"><span data-stu-id="cd9ed-176">Notes</span></span>|<span data-ttu-id="cd9ed-177">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-177">String</span></span>|<span data-ttu-id="cd9ed-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-178">Notes for the app.</span></span> <span data-ttu-id="cd9ed-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd9ed-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd9ed-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="cd9ed-180">publishingState</span></span>|<span data-ttu-id="cd9ed-181">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-181">String</span></span>|<span data-ttu-id="cd9ed-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-182">The publishing state for the app.</span></span> <span data-ttu-id="cd9ed-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cd9ed-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cd9ed-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="cd9ed-185">appUrl</span></span>|<span data-ttu-id="cd9ed-186">String</span><span class="sxs-lookup"><span data-stu-id="cd9ed-186">String</span></span>|<span data-ttu-id="cd9ed-187">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-187">The web app URL.</span></span>|
|<span data-ttu-id="cd9ed-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="cd9ed-188">useManagedBrowser</span></span>|<span data-ttu-id="cd9ed-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd9ed-189">Boolean</span></span>|<span data-ttu-id="cd9ed-190">Определяет, нужно ли использовать Managed Browser.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="cd9ed-191">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="cd9ed-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd9ed-192">Response</span></span>
<span data-ttu-id="cd9ed-193">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune_apps_webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-193">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9ed-194">Пример</span><span class="sxs-lookup"><span data-stu-id="cd9ed-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd9ed-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9ed-195">Request</span></span>
<span data-ttu-id="cd9ed-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 709

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

### <a name="response"></a><span data-ttu-id="cd9ed-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd9ed-197">Response</span></span>
<span data-ttu-id="cd9ed-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cd9ed-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



