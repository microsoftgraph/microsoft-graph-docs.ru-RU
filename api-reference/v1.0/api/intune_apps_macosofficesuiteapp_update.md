# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="db5d0-101">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="db5d0-101">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="db5d0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="db5d0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db5d0-103">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-103">Update the properties of a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db5d0-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="db5d0-104">Prerequisites</span></span>
<span data-ttu-id="db5d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db5d0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db5d0-107">Permission type</span></span>|<span data-ttu-id="db5d0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db5d0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db5d0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db5d0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="db5d0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5d0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db5d0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db5d0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db5d0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5d0-112">Not supported.</span></span>|
|<span data-ttu-id="db5d0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db5d0-113">Application</span></span>|<span data-ttu-id="db5d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5d0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db5d0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db5d0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="db5d0-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db5d0-116">Request headers</span></span>
|<span data-ttu-id="db5d0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db5d0-117">Header</span></span>|<span data-ttu-id="db5d0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="db5d0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db5d0-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db5d0-119">Authorization</span></span>|<span data-ttu-id="db5d0-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="db5d0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db5d0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="db5d0-121">Accept</span></span>|<span data-ttu-id="db5d0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="db5d0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db5d0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db5d0-123">Request body</span></span>
<span data-ttu-id="db5d0-124">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db5d0-124">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="db5d0-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-125">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="db5d0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="db5d0-126">Property</span></span>|<span data-ttu-id="db5d0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="db5d0-127">Type</span></span>|<span data-ttu-id="db5d0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="db5d0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db5d0-129">id</span><span class="sxs-lookup"><span data-stu-id="db5d0-129">id</span></span>|<span data-ttu-id="db5d0-130">Строка</span><span class="sxs-lookup"><span data-stu-id="db5d0-130">String</span></span>|<span data-ttu-id="db5d0-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="db5d0-131">Key of the entity.</span></span> <span data-ttu-id="db5d0-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="db5d0-133">displayName</span></span>|<span data-ttu-id="db5d0-134">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-134">String</span></span>|<span data-ttu-id="db5d0-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="db5d0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="db5d0-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-137">description</span><span class="sxs-lookup"><span data-stu-id="db5d0-137">description</span></span>|<span data-ttu-id="db5d0-138">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-138">String</span></span>|<span data-ttu-id="db5d0-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-139">The description of the app.</span></span> <span data-ttu-id="db5d0-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-141">publisher</span><span class="sxs-lookup"><span data-stu-id="db5d0-141">publisher</span></span>|<span data-ttu-id="db5d0-142">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-142">String</span></span>|<span data-ttu-id="db5d0-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-143">The publisher of the app.</span></span> <span data-ttu-id="db5d0-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="db5d0-145">largeIcon</span></span>|[<span data-ttu-id="db5d0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="db5d0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="db5d0-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="db5d0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="db5d0-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db5d0-149">createdDateTime</span></span>|<span data-ttu-id="db5d0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db5d0-150">DateTimeOffset</span></span>|<span data-ttu-id="db5d0-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-151">The date and time the app was created.</span></span> <span data-ttu-id="db5d0-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db5d0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="db5d0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db5d0-154">DateTimeOffset</span></span>|<span data-ttu-id="db5d0-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="db5d0-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="db5d0-157">isFeatured</span></span>|<span data-ttu-id="db5d0-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="db5d0-158">Boolean</span></span>|<span data-ttu-id="db5d0-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="db5d0-160">privacyInformationUrl</span></span>|<span data-ttu-id="db5d0-161">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-161">String</span></span>|<span data-ttu-id="db5d0-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="db5d0-162">The privacy statement Url.</span></span> <span data-ttu-id="db5d0-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="db5d0-164">informationUrl</span></span>|<span data-ttu-id="db5d0-165">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-165">String</span></span>|<span data-ttu-id="db5d0-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="db5d0-166">The more information Url.</span></span> <span data-ttu-id="db5d0-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-168">owner</span><span class="sxs-lookup"><span data-stu-id="db5d0-168">owner</span></span>|<span data-ttu-id="db5d0-169">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-169">String</span></span>|<span data-ttu-id="db5d0-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-170">The owner of the app.</span></span> <span data-ttu-id="db5d0-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-172">developer</span><span class="sxs-lookup"><span data-stu-id="db5d0-172">developer</span></span>|<span data-ttu-id="db5d0-173">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-173">String</span></span>|<span data-ttu-id="db5d0-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-174">The developer of the app.</span></span> <span data-ttu-id="db5d0-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-176">notes</span><span class="sxs-lookup"><span data-stu-id="db5d0-176">notes</span></span>|<span data-ttu-id="db5d0-177">String</span><span class="sxs-lookup"><span data-stu-id="db5d0-177">String</span></span>|<span data-ttu-id="db5d0-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="db5d0-178">Notes for the app.</span></span> <span data-ttu-id="db5d0-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="db5d0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="db5d0-180">publishingState</span></span>|[<span data-ttu-id="db5d0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="db5d0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="db5d0-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="db5d0-182">The publishing state for the app.</span></span> <span data-ttu-id="db5d0-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="db5d0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="db5d0-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db5d0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="db5d0-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="db5d0-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="db5d0-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="db5d0-186">Response</span></span>
<span data-ttu-id="db5d0-187">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db5d0-187">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db5d0-188">Пример</span><span class="sxs-lookup"><span data-stu-id="db5d0-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="db5d0-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="db5d0-189">Request</span></span>
<span data-ttu-id="db5d0-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db5d0-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 590

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="db5d0-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="db5d0-191">Response</span></span>
<span data-ttu-id="db5d0-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db5d0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```



