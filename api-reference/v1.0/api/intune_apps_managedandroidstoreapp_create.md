# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="f07d1-101">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f07d1-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="f07d1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f07d1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f07d1-103">Создание нового объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f07d1-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f07d1-104">Prerequisites</span></span>
<span data-ttu-id="f07d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f07d1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f07d1-107">Permission type</span></span>|<span data-ttu-id="f07d1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f07d1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f07d1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f07d1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f07d1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f07d1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f07d1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f07d1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f07d1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f07d1-112">Not supported.</span></span>|
|<span data-ttu-id="f07d1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f07d1-113">Application</span></span>|<span data-ttu-id="f07d1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f07d1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f07d1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f07d1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f07d1-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f07d1-116">Request headers</span></span>
|<span data-ttu-id="f07d1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f07d1-117">Header</span></span>|<span data-ttu-id="f07d1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f07d1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f07d1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f07d1-119">Authorization</span></span>|<span data-ttu-id="f07d1-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f07d1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f07d1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f07d1-121">Accept</span></span>|<span data-ttu-id="f07d1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f07d1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f07d1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f07d1-123">Request body</span></span>
<span data-ttu-id="f07d1-124">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f07d1-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f07d1-125">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="f07d1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f07d1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f07d1-126">Property</span></span>|<span data-ttu-id="f07d1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f07d1-127">Type</span></span>|<span data-ttu-id="f07d1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f07d1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f07d1-129">id</span><span class="sxs-lookup"><span data-stu-id="f07d1-129">id</span></span>|<span data-ttu-id="f07d1-130">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-130">String</span></span>|<span data-ttu-id="f07d1-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f07d1-131">Key of the setting.</span></span> <span data-ttu-id="f07d1-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f07d1-133">displayName</span></span>|<span data-ttu-id="f07d1-134">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-134">String</span></span>|<span data-ttu-id="f07d1-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f07d1-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f07d1-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-137">description</span><span class="sxs-lookup"><span data-stu-id="f07d1-137">description</span></span>|<span data-ttu-id="f07d1-138">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-138">String</span></span>|<span data-ttu-id="f07d1-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-139">The description of the app.</span></span> <span data-ttu-id="f07d1-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-141">publisher</span><span class="sxs-lookup"><span data-stu-id="f07d1-141">Publisher</span></span>|<span data-ttu-id="f07d1-142">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-142">String</span></span>|<span data-ttu-id="f07d1-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-143">The name of the app.</span></span> <span data-ttu-id="f07d1-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f07d1-145">largeIcon</span></span>|[<span data-ttu-id="f07d1-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f07d1-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="f07d1-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f07d1-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f07d1-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f07d1-149">createdDateTime</span></span>|<span data-ttu-id="f07d1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f07d1-150">DateTimeOffset</span></span>|<span data-ttu-id="f07d1-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-151">The date and time the group was created.</span></span> <span data-ttu-id="f07d1-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f07d1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f07d1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f07d1-154">DateTimeOffset</span></span>|<span data-ttu-id="f07d1-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="f07d1-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f07d1-157">isFeatured</span></span>|<span data-ttu-id="f07d1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f07d1-158">Boolean</span></span>|<span data-ttu-id="f07d1-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f07d1-160">privacyInformationUrl</span></span>|<span data-ttu-id="f07d1-161">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-161">String</span></span>|<span data-ttu-id="f07d1-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f07d1-162">The privacy statement Url.</span></span> <span data-ttu-id="f07d1-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f07d1-164">informationUrl</span></span>|<span data-ttu-id="f07d1-165">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-165">String</span></span>|<span data-ttu-id="f07d1-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f07d1-166">The more information Url.</span></span> <span data-ttu-id="f07d1-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-168">owner</span><span class="sxs-lookup"><span data-stu-id="f07d1-168">owner</span></span>|<span data-ttu-id="f07d1-169">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-169">String</span></span>|<span data-ttu-id="f07d1-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-170">The owner of the app.</span></span> <span data-ttu-id="f07d1-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-172">developer</span><span class="sxs-lookup"><span data-stu-id="f07d1-172">developer</span></span>|<span data-ttu-id="f07d1-173">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-173">String</span></span>|<span data-ttu-id="f07d1-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-174">The name of the app.</span></span> <span data-ttu-id="f07d1-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-176">notes</span><span class="sxs-lookup"><span data-stu-id="f07d1-176">Notes</span></span>|<span data-ttu-id="f07d1-177">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-177">String</span></span>|<span data-ttu-id="f07d1-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-178">Notes for the app.</span></span> <span data-ttu-id="f07d1-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f07d1-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f07d1-180">publishingState</span></span>|<span data-ttu-id="f07d1-181">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-181">String</span></span>|<span data-ttu-id="f07d1-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-182">The publishing state for the app.</span></span> <span data-ttu-id="f07d1-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f07d1-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f07d1-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f07d1-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f07d1-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f07d1-185">appAvailability</span></span>|<span data-ttu-id="f07d1-186">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-186">String</span></span>|<span data-ttu-id="f07d1-187">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-187">The Application's availability.</span></span> <span data-ttu-id="f07d1-188">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f07d1-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f07d1-189">version</span><span class="sxs-lookup"><span data-stu-id="f07d1-189">version</span></span>|<span data-ttu-id="f07d1-190">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-190">String</span></span>|<span data-ttu-id="f07d1-191">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-191">The Application's version.</span></span> <span data-ttu-id="f07d1-192">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f07d1-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="f07d1-193">packageId</span><span class="sxs-lookup"><span data-stu-id="f07d1-193">packageId</span></span>|<span data-ttu-id="f07d1-194">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-194">String</span></span>|<span data-ttu-id="f07d1-195">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="f07d1-195">The app's package ID.</span></span>|
|<span data-ttu-id="f07d1-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f07d1-196">appStoreUrl</span></span>|<span data-ttu-id="f07d1-197">String</span><span class="sxs-lookup"><span data-stu-id="f07d1-197">String</span></span>|<span data-ttu-id="f07d1-198">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="f07d1-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="f07d1-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f07d1-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f07d1-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f07d1-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="f07d1-201">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f07d1-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f07d1-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="f07d1-202">Response</span></span>
<span data-ttu-id="f07d1-203">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f07d1-203">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f07d1-204">Пример</span><span class="sxs-lookup"><span data-stu-id="f07d1-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="f07d1-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="f07d1-205">Request</span></span>
<span data-ttu-id="f07d1-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f07d1-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1080

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="f07d1-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="f07d1-207">Response</span></span>
<span data-ttu-id="f07d1-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f07d1-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



