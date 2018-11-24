# <a name="create-androidstoreapp"></a><span data-ttu-id="262af-101">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="262af-101">Create androidStoreApp</span></span>

> <span data-ttu-id="262af-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="262af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="262af-103">Создание объекта [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="262af-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="262af-104">Prerequisites</span></span>
<span data-ttu-id="262af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="262af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="262af-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="262af-107">Permission type</span></span>|<span data-ttu-id="262af-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="262af-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="262af-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="262af-109">Delegated (work or school account)</span></span>|<span data-ttu-id="262af-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262af-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="262af-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="262af-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="262af-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="262af-112">Not supported.</span></span>|
|<span data-ttu-id="262af-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="262af-113">Application</span></span>|<span data-ttu-id="262af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="262af-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="262af-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="262af-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="262af-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="262af-116">Request headers</span></span>
|<span data-ttu-id="262af-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="262af-117">Header</span></span>|<span data-ttu-id="262af-118">Значение</span><span class="sxs-lookup"><span data-stu-id="262af-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="262af-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="262af-119">Authorization</span></span>|<span data-ttu-id="262af-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="262af-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="262af-121">Accept</span><span class="sxs-lookup"><span data-stu-id="262af-121">Accept</span></span>|<span data-ttu-id="262af-122">application/json</span><span class="sxs-lookup"><span data-stu-id="262af-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="262af-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="262af-123">Request body</span></span>
<span data-ttu-id="262af-124">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="262af-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="262af-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="262af-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="262af-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="262af-126">Property</span></span>|<span data-ttu-id="262af-127">Тип</span><span class="sxs-lookup"><span data-stu-id="262af-127">Type</span></span>|<span data-ttu-id="262af-128">Описание</span><span class="sxs-lookup"><span data-stu-id="262af-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="262af-129">id</span><span class="sxs-lookup"><span data-stu-id="262af-129">id</span></span>|<span data-ttu-id="262af-130">String</span><span class="sxs-lookup"><span data-stu-id="262af-130">String</span></span>|<span data-ttu-id="262af-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="262af-131">Key of the entity.</span></span> <span data-ttu-id="262af-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-133">displayName</span><span class="sxs-lookup"><span data-stu-id="262af-133">displayName</span></span>|<span data-ttu-id="262af-134">String</span><span class="sxs-lookup"><span data-stu-id="262af-134">String</span></span>|<span data-ttu-id="262af-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="262af-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="262af-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-137">description</span><span class="sxs-lookup"><span data-stu-id="262af-137">description</span></span>|<span data-ttu-id="262af-138">String</span><span class="sxs-lookup"><span data-stu-id="262af-138">String</span></span>|<span data-ttu-id="262af-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-139">The description of the app.</span></span> <span data-ttu-id="262af-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-141">publisher</span><span class="sxs-lookup"><span data-stu-id="262af-141">publisher</span></span>|<span data-ttu-id="262af-142">String</span><span class="sxs-lookup"><span data-stu-id="262af-142">String</span></span>|<span data-ttu-id="262af-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-143">The publisher of the app.</span></span> <span data-ttu-id="262af-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="262af-145">largeIcon</span></span>|[<span data-ttu-id="262af-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="262af-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="262af-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="262af-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="262af-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="262af-149">createdDateTime</span></span>|<span data-ttu-id="262af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="262af-150">DateTimeOffset</span></span>|<span data-ttu-id="262af-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-151">The date and time the app was created.</span></span> <span data-ttu-id="262af-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="262af-153">lastModifiedDateTime</span></span>|<span data-ttu-id="262af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="262af-154">DateTimeOffset</span></span>|<span data-ttu-id="262af-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-155">The date and time the app was last modified.</span></span> <span data-ttu-id="262af-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="262af-157">isFeatured</span></span>|<span data-ttu-id="262af-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="262af-158">Boolean</span></span>|<span data-ttu-id="262af-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="262af-160">privacyInformationUrl</span></span>|<span data-ttu-id="262af-161">String</span><span class="sxs-lookup"><span data-stu-id="262af-161">String</span></span>|<span data-ttu-id="262af-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="262af-162">The privacy statement Url.</span></span> <span data-ttu-id="262af-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="262af-164">informationUrl</span></span>|<span data-ttu-id="262af-165">String</span><span class="sxs-lookup"><span data-stu-id="262af-165">String</span></span>|<span data-ttu-id="262af-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="262af-166">The more information Url.</span></span> <span data-ttu-id="262af-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-168">owner</span><span class="sxs-lookup"><span data-stu-id="262af-168">owner</span></span>|<span data-ttu-id="262af-169">String</span><span class="sxs-lookup"><span data-stu-id="262af-169">String</span></span>|<span data-ttu-id="262af-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-170">The owner of the app.</span></span> <span data-ttu-id="262af-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-172">developer</span><span class="sxs-lookup"><span data-stu-id="262af-172">developer</span></span>|<span data-ttu-id="262af-173">String</span><span class="sxs-lookup"><span data-stu-id="262af-173">String</span></span>|<span data-ttu-id="262af-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-174">The developer of the app.</span></span> <span data-ttu-id="262af-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-176">notes</span><span class="sxs-lookup"><span data-stu-id="262af-176">notes</span></span>|<span data-ttu-id="262af-177">String</span><span class="sxs-lookup"><span data-stu-id="262af-177">String</span></span>|<span data-ttu-id="262af-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-178">Notes for the app.</span></span> <span data-ttu-id="262af-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="262af-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="262af-180">publishingState</span></span>|[<span data-ttu-id="262af-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="262af-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="262af-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="262af-182">The publishing state for the app.</span></span> <span data-ttu-id="262af-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="262af-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="262af-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="262af-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="262af-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="262af-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="262af-186">packageId</span><span class="sxs-lookup"><span data-stu-id="262af-186">packageId</span></span>|<span data-ttu-id="262af-187">String</span><span class="sxs-lookup"><span data-stu-id="262af-187">String</span></span>|<span data-ttu-id="262af-188">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="262af-188">The package identifier.</span></span>|
|<span data-ttu-id="262af-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="262af-189">appStoreUrl</span></span>|<span data-ttu-id="262af-190">String</span><span class="sxs-lookup"><span data-stu-id="262af-190">String</span></span>|<span data-ttu-id="262af-191">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="262af-191">The Android app store URL.</span></span>|
|<span data-ttu-id="262af-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="262af-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="262af-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="262af-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="262af-194">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="262af-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="262af-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="262af-195">Response</span></span>
<span data-ttu-id="262af-196">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune_apps_androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="262af-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="262af-197">Пример</span><span class="sxs-lookup"><span data-stu-id="262af-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="262af-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="262af-198">Request</span></span>
<span data-ttu-id="262af-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="262af-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="262af-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="262af-200">Response</span></span>
<span data-ttu-id="262af-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="262af-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```



