# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="56aa3-101">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="56aa3-101">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="56aa3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56aa3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56aa3-103">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-103">Update the properties of a [calendar](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56aa3-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="56aa3-104">Prerequisites</span></span>
<span data-ttu-id="56aa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56aa3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56aa3-107">Permission type</span></span>|<span data-ttu-id="56aa3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56aa3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56aa3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56aa3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56aa3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56aa3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56aa3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56aa3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56aa3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56aa3-112">Not supported.</span></span>|
|<span data-ttu-id="56aa3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56aa3-113">Application</span></span>|<span data-ttu-id="56aa3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56aa3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56aa3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56aa3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="56aa3-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="56aa3-116">Request headers</span></span>
|<span data-ttu-id="56aa3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56aa3-117">Header</span></span>|<span data-ttu-id="56aa3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="56aa3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56aa3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="56aa3-119">Authorization</span></span>|<span data-ttu-id="56aa3-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56aa3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56aa3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="56aa3-121">Accept</span></span>|<span data-ttu-id="56aa3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="56aa3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56aa3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56aa3-123">Request body</span></span>
<span data-ttu-id="56aa3-124">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56aa3-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="56aa3-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="56aa3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="56aa3-126">Property</span></span>|<span data-ttu-id="56aa3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="56aa3-127">Type</span></span>|<span data-ttu-id="56aa3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="56aa3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56aa3-129">id</span><span class="sxs-lookup"><span data-stu-id="56aa3-129">id</span></span>|<span data-ttu-id="56aa3-130">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-130">String</span></span>|<span data-ttu-id="56aa3-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="56aa3-131">Key of the setting.</span></span> <span data-ttu-id="56aa3-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="56aa3-133">displayName</span></span>|<span data-ttu-id="56aa3-134">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-134">String</span></span>|<span data-ttu-id="56aa3-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="56aa3-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="56aa3-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-137">description</span><span class="sxs-lookup"><span data-stu-id="56aa3-137">description</span></span>|<span data-ttu-id="56aa3-138">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-138">String</span></span>|<span data-ttu-id="56aa3-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-139">The description of the app.</span></span> <span data-ttu-id="56aa3-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-141">publisher</span><span class="sxs-lookup"><span data-stu-id="56aa3-141">Publisher</span></span>|<span data-ttu-id="56aa3-142">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-142">String</span></span>|<span data-ttu-id="56aa3-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-143">The name of the app.</span></span> <span data-ttu-id="56aa3-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="56aa3-145">largeIcon</span></span>|[<span data-ttu-id="56aa3-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="56aa3-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="56aa3-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="56aa3-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="56aa3-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56aa3-149">createdDateTime</span></span>|<span data-ttu-id="56aa3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aa3-150">DateTimeOffset</span></span>|<span data-ttu-id="56aa3-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-151">The date and time the group was created.</span></span> <span data-ttu-id="56aa3-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56aa3-153">lastModifiedDateTime</span></span>|<span data-ttu-id="56aa3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aa3-154">DateTimeOffset</span></span>|<span data-ttu-id="56aa3-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="56aa3-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="56aa3-157">isFeatured</span></span>|<span data-ttu-id="56aa3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="56aa3-158">Boolean</span></span>|<span data-ttu-id="56aa3-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="56aa3-160">privacyInformationUrl</span></span>|<span data-ttu-id="56aa3-161">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-161">String</span></span>|<span data-ttu-id="56aa3-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="56aa3-162">The privacy statement Url.</span></span> <span data-ttu-id="56aa3-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="56aa3-164">informationUrl</span></span>|<span data-ttu-id="56aa3-165">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-165">String</span></span>|<span data-ttu-id="56aa3-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="56aa3-166">The more information Url.</span></span> <span data-ttu-id="56aa3-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-168">owner</span><span class="sxs-lookup"><span data-stu-id="56aa3-168">owner</span></span>|<span data-ttu-id="56aa3-169">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-169">String</span></span>|<span data-ttu-id="56aa3-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-170">The owner of the app.</span></span> <span data-ttu-id="56aa3-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-172">developer</span><span class="sxs-lookup"><span data-stu-id="56aa3-172">developer</span></span>|<span data-ttu-id="56aa3-173">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-173">String</span></span>|<span data-ttu-id="56aa3-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-174">The name of the app.</span></span> <span data-ttu-id="56aa3-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-176">notes</span><span class="sxs-lookup"><span data-stu-id="56aa3-176">Notes</span></span>|<span data-ttu-id="56aa3-177">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-177">String</span></span>|<span data-ttu-id="56aa3-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-178">Notes for the app.</span></span> <span data-ttu-id="56aa3-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="56aa3-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="56aa3-180">publishingState</span></span>|<span data-ttu-id="56aa3-181">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-181">String</span></span>|<span data-ttu-id="56aa3-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-182">The publishing state for the app.</span></span> <span data-ttu-id="56aa3-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="56aa3-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="56aa3-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="56aa3-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="56aa3-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="56aa3-185">appAvailability</span></span>|<span data-ttu-id="56aa3-186">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-186">String</span></span>|<span data-ttu-id="56aa3-187">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-187">The Application's availability.</span></span> <span data-ttu-id="56aa3-188">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="56aa3-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="56aa3-189">version</span><span class="sxs-lookup"><span data-stu-id="56aa3-189">version</span></span>|<span data-ttu-id="56aa3-190">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-190">String</span></span>|<span data-ttu-id="56aa3-191">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-191">The Application's version.</span></span> <span data-ttu-id="56aa3-192">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="56aa3-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="56aa3-193">packageId</span><span class="sxs-lookup"><span data-stu-id="56aa3-193">packageId</span></span>|<span data-ttu-id="56aa3-194">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-194">String</span></span>|<span data-ttu-id="56aa3-195">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="56aa3-195">The app's package ID.</span></span>|
|<span data-ttu-id="56aa3-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="56aa3-196">appStoreUrl</span></span>|<span data-ttu-id="56aa3-197">String</span><span class="sxs-lookup"><span data-stu-id="56aa3-197">String</span></span>|<span data-ttu-id="56aa3-198">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="56aa3-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="56aa3-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56aa3-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="56aa3-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56aa3-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="56aa3-201">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="56aa3-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="56aa3-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="56aa3-202">Response</span></span>
<span data-ttu-id="56aa3-203">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56aa3-203">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56aa3-204">Пример</span><span class="sxs-lookup"><span data-stu-id="56aa3-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="56aa3-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="56aa3-205">Request</span></span>
<span data-ttu-id="56aa3-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56aa3-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1019

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

### <a name="response"></a><span data-ttu-id="56aa3-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="56aa3-207">Response</span></span>
<span data-ttu-id="56aa3-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56aa3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



