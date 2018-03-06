# <a name="update-androidstoreapp"></a><span data-ttu-id="548bd-101">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="548bd-101">Update androidStoreApp</span></span>

> <span data-ttu-id="548bd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="548bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="548bd-103">Обновление свойств объекта [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-103">Update the properties of a [calendar](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="548bd-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="548bd-104">Prerequisites</span></span>
<span data-ttu-id="548bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="548bd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="548bd-107">Permission type</span></span>|<span data-ttu-id="548bd-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="548bd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="548bd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="548bd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="548bd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="548bd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="548bd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="548bd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="548bd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="548bd-112">Not supported.</span></span>|
|<span data-ttu-id="548bd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="548bd-113">Application</span></span>|<span data-ttu-id="548bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="548bd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="548bd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="548bd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="548bd-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="548bd-116">Request headers</span></span>
|<span data-ttu-id="548bd-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="548bd-117">Header</span></span>|<span data-ttu-id="548bd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="548bd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="548bd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="548bd-119">Authorization</span></span>|<span data-ttu-id="548bd-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="548bd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="548bd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="548bd-121">Accept</span></span>|<span data-ttu-id="548bd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="548bd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="548bd-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="548bd-123">Request body</span></span>
<span data-ttu-id="548bd-124">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune_apps_androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="548bd-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_androidstoreapp.md) object.</span></span>

<span data-ttu-id="548bd-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="548bd-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="548bd-126">Property</span></span>|<span data-ttu-id="548bd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="548bd-127">Type</span></span>|<span data-ttu-id="548bd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="548bd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="548bd-129">id</span><span class="sxs-lookup"><span data-stu-id="548bd-129">id</span></span>|<span data-ttu-id="548bd-130">String</span><span class="sxs-lookup"><span data-stu-id="548bd-130">String</span></span>|<span data-ttu-id="548bd-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="548bd-131">Key of the setting.</span></span> <span data-ttu-id="548bd-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="548bd-133">displayName</span></span>|<span data-ttu-id="548bd-134">String</span><span class="sxs-lookup"><span data-stu-id="548bd-134">String</span></span>|<span data-ttu-id="548bd-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="548bd-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="548bd-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-137">description</span><span class="sxs-lookup"><span data-stu-id="548bd-137">description</span></span>|<span data-ttu-id="548bd-138">String</span><span class="sxs-lookup"><span data-stu-id="548bd-138">String</span></span>|<span data-ttu-id="548bd-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-139">The description of the app.</span></span> <span data-ttu-id="548bd-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-141">publisher</span><span class="sxs-lookup"><span data-stu-id="548bd-141">Publisher</span></span>|<span data-ttu-id="548bd-142">String</span><span class="sxs-lookup"><span data-stu-id="548bd-142">String</span></span>|<span data-ttu-id="548bd-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-143">The name of the app.</span></span> <span data-ttu-id="548bd-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="548bd-145">largeIcon</span></span>|[<span data-ttu-id="548bd-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="548bd-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="548bd-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="548bd-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="548bd-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="548bd-149">createdDateTime</span></span>|<span data-ttu-id="548bd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548bd-150">DateTimeOffset</span></span>|<span data-ttu-id="548bd-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-151">The date and time the group was created.</span></span> <span data-ttu-id="548bd-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="548bd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="548bd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548bd-154">DateTimeOffset</span></span>|<span data-ttu-id="548bd-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="548bd-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="548bd-157">isFeatured</span></span>|<span data-ttu-id="548bd-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="548bd-158">Boolean</span></span>|<span data-ttu-id="548bd-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="548bd-160">privacyInformationUrl</span></span>|<span data-ttu-id="548bd-161">String</span><span class="sxs-lookup"><span data-stu-id="548bd-161">String</span></span>|<span data-ttu-id="548bd-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="548bd-162">The privacy statement Url.</span></span> <span data-ttu-id="548bd-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="548bd-164">informationUrl</span></span>|<span data-ttu-id="548bd-165">String</span><span class="sxs-lookup"><span data-stu-id="548bd-165">String</span></span>|<span data-ttu-id="548bd-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="548bd-166">The more information Url.</span></span> <span data-ttu-id="548bd-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-168">owner</span><span class="sxs-lookup"><span data-stu-id="548bd-168">owner</span></span>|<span data-ttu-id="548bd-169">String</span><span class="sxs-lookup"><span data-stu-id="548bd-169">String</span></span>|<span data-ttu-id="548bd-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-170">The owner of the app.</span></span> <span data-ttu-id="548bd-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-172">developer</span><span class="sxs-lookup"><span data-stu-id="548bd-172">developer</span></span>|<span data-ttu-id="548bd-173">String</span><span class="sxs-lookup"><span data-stu-id="548bd-173">String</span></span>|<span data-ttu-id="548bd-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-174">The name of the app.</span></span> <span data-ttu-id="548bd-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-176">notes</span><span class="sxs-lookup"><span data-stu-id="548bd-176">Notes</span></span>|<span data-ttu-id="548bd-177">String</span><span class="sxs-lookup"><span data-stu-id="548bd-177">String</span></span>|<span data-ttu-id="548bd-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-178">Notes for the app.</span></span> <span data-ttu-id="548bd-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="548bd-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="548bd-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="548bd-180">publishingState</span></span>|<span data-ttu-id="548bd-181">String</span><span class="sxs-lookup"><span data-stu-id="548bd-181">String</span></span>|<span data-ttu-id="548bd-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="548bd-182">The publishing state for the app.</span></span> <span data-ttu-id="548bd-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="548bd-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="548bd-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="548bd-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="548bd-185">packageId</span><span class="sxs-lookup"><span data-stu-id="548bd-185">packageId</span></span>|<span data-ttu-id="548bd-186">String</span><span class="sxs-lookup"><span data-stu-id="548bd-186">String</span></span>|<span data-ttu-id="548bd-187">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="548bd-187">The package identifier.</span></span>|
|<span data-ttu-id="548bd-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="548bd-188">appStoreUrl</span></span>|<span data-ttu-id="548bd-189">String</span><span class="sxs-lookup"><span data-stu-id="548bd-189">String</span></span>|<span data-ttu-id="548bd-190">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="548bd-190">The Android app store URL.</span></span>|
|<span data-ttu-id="548bd-191">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="548bd-191">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="548bd-192">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="548bd-192">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="548bd-193">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="548bd-193">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="548bd-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="548bd-194">Response</span></span>
<span data-ttu-id="548bd-195">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune_apps_androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="548bd-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="548bd-196">Пример</span><span class="sxs-lookup"><span data-stu-id="548bd-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="548bd-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="548bd-197">Request</span></span>
<span data-ttu-id="548bd-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="548bd-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 948

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

### <a name="response"></a><span data-ttu-id="548bd-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="548bd-199">Response</span></span>
<span data-ttu-id="548bd-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="548bd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



