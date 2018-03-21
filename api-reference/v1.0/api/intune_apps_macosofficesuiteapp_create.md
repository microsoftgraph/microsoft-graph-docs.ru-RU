# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="ab7e9-101">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="ab7e9-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="ab7e9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab7e9-103">Создание объекта [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-103">Create a new [plannerBucket](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab7e9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab7e9-104">Prerequisites</span></span>
<span data-ttu-id="ab7e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab7e9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab7e9-107">Permission type</span></span>|<span data-ttu-id="ab7e9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab7e9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab7e9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab7e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ab7e9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab7e9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab7e9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab7e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab7e9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-112">Not supported.</span></span>|
|<span data-ttu-id="ab7e9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab7e9-113">Application</span></span>|<span data-ttu-id="ab7e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab7e9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab7e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ab7e9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab7e9-116">Request headers</span></span>
|<span data-ttu-id="ab7e9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab7e9-117">Header</span></span>|<span data-ttu-id="ab7e9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ab7e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab7e9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab7e9-119">Authorization</span></span>|<span data-ttu-id="ab7e9-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ab7e9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ab7e9-121">Accept</span></span>|<span data-ttu-id="ab7e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ab7e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab7e9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab7e9-123">Request body</span></span>
<span data-ttu-id="ab7e9-124">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ab7e9-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ab7e9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab7e9-126">Property</span></span>|<span data-ttu-id="ab7e9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ab7e9-127">Type</span></span>|<span data-ttu-id="ab7e9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ab7e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7e9-129">id</span><span class="sxs-lookup"><span data-stu-id="ab7e9-129">id</span></span>|<span data-ttu-id="ab7e9-130">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-130">String</span></span>|<span data-ttu-id="ab7e9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-131">Key of the setting.</span></span> <span data-ttu-id="ab7e9-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ab7e9-133">displayName</span></span>|<span data-ttu-id="ab7e9-134">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-134">String</span></span>|<span data-ttu-id="ab7e9-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ab7e9-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-137">description</span><span class="sxs-lookup"><span data-stu-id="ab7e9-137">description</span></span>|<span data-ttu-id="ab7e9-138">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-138">String</span></span>|<span data-ttu-id="ab7e9-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-139">The description of the app.</span></span> <span data-ttu-id="ab7e9-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ab7e9-141">Publisher</span></span>|<span data-ttu-id="ab7e9-142">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-142">String</span></span>|<span data-ttu-id="ab7e9-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-143">The name of the app.</span></span> <span data-ttu-id="ab7e9-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ab7e9-145">largeIcon</span></span>|[<span data-ttu-id="ab7e9-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ab7e9-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ab7e9-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ab7e9-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab7e9-149">createdDateTime</span></span>|<span data-ttu-id="ab7e9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab7e9-150">DateTimeOffset</span></span>|<span data-ttu-id="ab7e9-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-151">The date and time the group was created.</span></span> <span data-ttu-id="ab7e9-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab7e9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ab7e9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab7e9-154">DateTimeOffset</span></span>|<span data-ttu-id="ab7e9-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ab7e9-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ab7e9-157">isFeatured</span></span>|<span data-ttu-id="ab7e9-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab7e9-158">Boolean</span></span>|<span data-ttu-id="ab7e9-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ab7e9-160">privacyInformationUrl</span></span>|<span data-ttu-id="ab7e9-161">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-161">String</span></span>|<span data-ttu-id="ab7e9-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-162">The privacy statement Url.</span></span> <span data-ttu-id="ab7e9-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ab7e9-164">informationUrl</span></span>|<span data-ttu-id="ab7e9-165">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-165">String</span></span>|<span data-ttu-id="ab7e9-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-166">The more information Url.</span></span> <span data-ttu-id="ab7e9-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-168">owner</span><span class="sxs-lookup"><span data-stu-id="ab7e9-168">owner</span></span>|<span data-ttu-id="ab7e9-169">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-169">String</span></span>|<span data-ttu-id="ab7e9-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-170">The owner of the app.</span></span> <span data-ttu-id="ab7e9-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-172">developer</span><span class="sxs-lookup"><span data-stu-id="ab7e9-172">developer</span></span>|<span data-ttu-id="ab7e9-173">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-173">String</span></span>|<span data-ttu-id="ab7e9-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-174">The name of the app.</span></span> <span data-ttu-id="ab7e9-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-176">notes</span><span class="sxs-lookup"><span data-stu-id="ab7e9-176">Notes</span></span>|<span data-ttu-id="ab7e9-177">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-177">String</span></span>|<span data-ttu-id="ab7e9-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-178">Notes for the app.</span></span> <span data-ttu-id="ab7e9-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ab7e9-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ab7e9-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ab7e9-180">publishingState</span></span>|<span data-ttu-id="ab7e9-181">String</span><span class="sxs-lookup"><span data-stu-id="ab7e9-181">String</span></span>|<span data-ttu-id="ab7e9-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-182">The publishing state for the app.</span></span> <span data-ttu-id="ab7e9-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ab7e9-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="ab7e9-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab7e9-185">Response</span></span>
<span data-ttu-id="ab7e9-186">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-186">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab7e9-187">Пример</span><span class="sxs-lookup"><span data-stu-id="ab7e9-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab7e9-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab7e9-188">Request</span></span>
<span data-ttu-id="ab7e9-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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

### <a name="response"></a><span data-ttu-id="ab7e9-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab7e9-190">Response</span></span>
<span data-ttu-id="ab7e9-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab7e9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



