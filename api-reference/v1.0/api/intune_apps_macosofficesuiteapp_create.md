# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="22f4c-101">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="22f4c-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="22f4c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22f4c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22f4c-103">Создание объекта [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-103">Create a new [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22f4c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="22f4c-104">Prerequisites</span></span>
<span data-ttu-id="22f4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22f4c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22f4c-107">Permission type</span></span>|<span data-ttu-id="22f4c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22f4c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f4c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22f4c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="22f4c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f4c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22f4c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22f4c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f4c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22f4c-112">Not supported.</span></span>|
|<span data-ttu-id="22f4c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22f4c-113">Application</span></span>|<span data-ttu-id="22f4c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22f4c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f4c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22f4c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="22f4c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22f4c-116">Request headers</span></span>
|<span data-ttu-id="22f4c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22f4c-117">Header</span></span>|<span data-ttu-id="22f4c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="22f4c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f4c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22f4c-119">Authorization</span></span>|<span data-ttu-id="22f4c-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="22f4c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f4c-121">Принять</span><span class="sxs-lookup"><span data-stu-id="22f4c-121">Accept</span></span>|<span data-ttu-id="22f4c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="22f4c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f4c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22f4c-123">Request body</span></span>
<span data-ttu-id="22f4c-124">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22f4c-124">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="22f4c-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="22f4c-125">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="22f4c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="22f4c-126">Property</span></span>|<span data-ttu-id="22f4c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="22f4c-127">Type</span></span>|<span data-ttu-id="22f4c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="22f4c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f4c-129">id</span><span class="sxs-lookup"><span data-stu-id="22f4c-129">id</span></span>|<span data-ttu-id="22f4c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-130">String</span></span>|<span data-ttu-id="22f4c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22f4c-131">Key of the entity.</span></span> <span data-ttu-id="22f4c-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="22f4c-133">displayName</span></span>|<span data-ttu-id="22f4c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-134">String</span></span>|<span data-ttu-id="22f4c-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="22f4c-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="22f4c-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-137">description</span><span class="sxs-lookup"><span data-stu-id="22f4c-137">description</span></span>|<span data-ttu-id="22f4c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-138">String</span></span>|<span data-ttu-id="22f4c-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-139">The description of the app.</span></span> <span data-ttu-id="22f4c-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-141">publisher</span><span class="sxs-lookup"><span data-stu-id="22f4c-141">publisher</span></span>|<span data-ttu-id="22f4c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-142">String</span></span>|<span data-ttu-id="22f4c-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-143">The publisher of the app.</span></span> <span data-ttu-id="22f4c-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22f4c-145">largeIcon</span></span>|[<span data-ttu-id="22f4c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22f4c-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="22f4c-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="22f4c-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="22f4c-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22f4c-149">createdDateTime</span></span>|<span data-ttu-id="22f4c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f4c-150">DateTimeOffset</span></span>|<span data-ttu-id="22f4c-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-151">The date and time the app was created.</span></span> <span data-ttu-id="22f4c-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22f4c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="22f4c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f4c-154">DateTimeOffset</span></span>|<span data-ttu-id="22f4c-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-155">The date and time the app was last modified.</span></span> <span data-ttu-id="22f4c-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22f4c-157">isFeatured</span></span>|<span data-ttu-id="22f4c-158">Логический</span><span class="sxs-lookup"><span data-stu-id="22f4c-158">Boolean</span></span>|<span data-ttu-id="22f4c-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22f4c-160">privacyInformationUrl</span></span>|<span data-ttu-id="22f4c-161">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-161">String</span></span>|<span data-ttu-id="22f4c-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="22f4c-162">The privacy statement Url.</span></span> <span data-ttu-id="22f4c-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22f4c-164">informationUrl</span></span>|<span data-ttu-id="22f4c-165">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-165">String</span></span>|<span data-ttu-id="22f4c-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="22f4c-166">The more information Url.</span></span> <span data-ttu-id="22f4c-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-168">owner</span><span class="sxs-lookup"><span data-stu-id="22f4c-168">owner</span></span>|<span data-ttu-id="22f4c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-169">String</span></span>|<span data-ttu-id="22f4c-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-170">The owner of the app.</span></span> <span data-ttu-id="22f4c-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-172">developer</span><span class="sxs-lookup"><span data-stu-id="22f4c-172">developer</span></span>|<span data-ttu-id="22f4c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-173">String</span></span>|<span data-ttu-id="22f4c-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-174">The developer of the app.</span></span> <span data-ttu-id="22f4c-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-176">notes</span><span class="sxs-lookup"><span data-stu-id="22f4c-176">notes</span></span>|<span data-ttu-id="22f4c-177">Строка</span><span class="sxs-lookup"><span data-stu-id="22f4c-177">String</span></span>|<span data-ttu-id="22f4c-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="22f4c-178">Notes for the app.</span></span> <span data-ttu-id="22f4c-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="22f4c-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="22f4c-180">publishingState</span></span>|[<span data-ttu-id="22f4c-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="22f4c-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="22f4c-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="22f4c-182">The publishing state for the app.</span></span> <span data-ttu-id="22f4c-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="22f4c-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22f4c-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22f4c-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="22f4c-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="22f4c-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="22f4c-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="22f4c-186">Response</span></span>
<span data-ttu-id="22f4c-187">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22f4c-187">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f4c-188">Пример</span><span class="sxs-lookup"><span data-stu-id="22f4c-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="22f4c-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="22f4c-189">Request</span></span>
<span data-ttu-id="22f4c-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22f4c-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22f4c-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="22f4c-191">Response</span></span>
<span data-ttu-id="22f4c-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22f4c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








