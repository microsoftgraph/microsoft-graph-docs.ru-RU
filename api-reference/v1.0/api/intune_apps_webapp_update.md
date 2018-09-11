# <a name="update-webapp"></a><span data-ttu-id="d2324-101">Обновление webApp</span><span class="sxs-lookup"><span data-stu-id="d2324-101">Update webApp</span></span>

> <span data-ttu-id="d2324-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2324-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2324-103">Обновление свойств объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-103">Update the properties of a [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2324-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d2324-104">Prerequisites</span></span>
<span data-ttu-id="d2324-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2324-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2324-107">Permission type</span></span>|<span data-ttu-id="d2324-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2324-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2324-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2324-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2324-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2324-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2324-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2324-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2324-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2324-112">Not supported.</span></span>|
|<span data-ttu-id="d2324-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2324-113">Application</span></span>|<span data-ttu-id="d2324-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2324-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2324-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2324-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d2324-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2324-116">Request headers</span></span>
|<span data-ttu-id="d2324-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2324-117">Header</span></span>|<span data-ttu-id="d2324-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d2324-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2324-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2324-119">Authorization</span></span>|<span data-ttu-id="d2324-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="d2324-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2324-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d2324-121">Accept</span></span>|<span data-ttu-id="d2324-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2324-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2324-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2324-123">Request body</span></span>
<span data-ttu-id="d2324-124">В тексте запроса добавьте представление объекта [webApp](../resources/intune_apps_webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2324-124">In the request body, supply a JSON representation for the [webApp](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="d2324-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-125">The following table shows the properties that are required when you create the [webApp](../resources/intune_apps_webapp.md).</span></span>

|<span data-ttu-id="d2324-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2324-126">Property</span></span>|<span data-ttu-id="d2324-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d2324-127">Type</span></span>|<span data-ttu-id="d2324-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d2324-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2324-129">id</span><span class="sxs-lookup"><span data-stu-id="d2324-129">id</span></span>|<span data-ttu-id="d2324-130">String</span><span class="sxs-lookup"><span data-stu-id="d2324-130">String</span></span>|<span data-ttu-id="d2324-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2324-131">Key of the entity.</span></span> <span data-ttu-id="d2324-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d2324-133">displayName</span></span>|<span data-ttu-id="d2324-134">String</span><span class="sxs-lookup"><span data-stu-id="d2324-134">String</span></span>|<span data-ttu-id="d2324-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d2324-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d2324-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-137">description</span><span class="sxs-lookup"><span data-stu-id="d2324-137">description</span></span>|<span data-ttu-id="d2324-138">String</span><span class="sxs-lookup"><span data-stu-id="d2324-138">String</span></span>|<span data-ttu-id="d2324-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-139">The description of the app.</span></span> <span data-ttu-id="d2324-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d2324-141">publisher</span></span>|<span data-ttu-id="d2324-142">String</span><span class="sxs-lookup"><span data-stu-id="d2324-142">String</span></span>|<span data-ttu-id="d2324-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-143">The publisher of the app.</span></span> <span data-ttu-id="d2324-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d2324-145">largeIcon</span></span>|[<span data-ttu-id="d2324-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d2324-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="d2324-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d2324-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d2324-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2324-149">createdDateTime</span></span>|<span data-ttu-id="d2324-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2324-150">DateTimeOffset</span></span>|<span data-ttu-id="d2324-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-151">The date and time the app was created.</span></span> <span data-ttu-id="d2324-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2324-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d2324-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2324-154">DateTimeOffset</span></span>|<span data-ttu-id="d2324-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-155">The date and time the app was last modified.</span></span> <span data-ttu-id="d2324-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d2324-157">isFeatured</span></span>|<span data-ttu-id="d2324-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2324-158">Boolean</span></span>|<span data-ttu-id="d2324-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d2324-160">privacyInformationUrl</span></span>|<span data-ttu-id="d2324-161">String</span><span class="sxs-lookup"><span data-stu-id="d2324-161">String</span></span>|<span data-ttu-id="d2324-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d2324-162">The privacy statement Url.</span></span> <span data-ttu-id="d2324-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d2324-164">informationUrl</span></span>|<span data-ttu-id="d2324-165">String</span><span class="sxs-lookup"><span data-stu-id="d2324-165">String</span></span>|<span data-ttu-id="d2324-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d2324-166">The more information Url.</span></span> <span data-ttu-id="d2324-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-168">owner</span><span class="sxs-lookup"><span data-stu-id="d2324-168">owner</span></span>|<span data-ttu-id="d2324-169">String</span><span class="sxs-lookup"><span data-stu-id="d2324-169">String</span></span>|<span data-ttu-id="d2324-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-170">The owner of the app.</span></span> <span data-ttu-id="d2324-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-172">developer</span><span class="sxs-lookup"><span data-stu-id="d2324-172">developer</span></span>|<span data-ttu-id="d2324-173">String</span><span class="sxs-lookup"><span data-stu-id="d2324-173">String</span></span>|<span data-ttu-id="d2324-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-174">The developer of the app.</span></span> <span data-ttu-id="d2324-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-176">notes</span><span class="sxs-lookup"><span data-stu-id="d2324-176">notes</span></span>|<span data-ttu-id="d2324-177">String</span><span class="sxs-lookup"><span data-stu-id="d2324-177">String</span></span>|<span data-ttu-id="d2324-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="d2324-178">Notes for the app.</span></span> <span data-ttu-id="d2324-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2324-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d2324-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d2324-180">publishingState</span></span>|[<span data-ttu-id="d2324-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d2324-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="d2324-p114">Состояние публикации для приложения. Приложение может быть назначено только в случае публикации приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d2324-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d2324-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="d2324-186">appUrl</span></span>|<span data-ttu-id="d2324-187">String</span><span class="sxs-lookup"><span data-stu-id="d2324-187">String</span></span>|<span data-ttu-id="d2324-188">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="d2324-188">The web app URL.</span></span>|
|<span data-ttu-id="d2324-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="d2324-189">useManagedBrowser</span></span>|<span data-ttu-id="d2324-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2324-190">Boolean</span></span>|<span data-ttu-id="d2324-191">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="d2324-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="d2324-192">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="d2324-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="d2324-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2324-193">Response</span></span>
<span data-ttu-id="d2324-194">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune_apps_webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2324-194">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2324-195">Пример</span><span class="sxs-lookup"><span data-stu-id="d2324-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2324-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2324-196">Request</span></span>
<span data-ttu-id="d2324-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2324-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 664

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="d2324-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2324-198">Response</span></span>
<span data-ttu-id="d2324-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2324-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








