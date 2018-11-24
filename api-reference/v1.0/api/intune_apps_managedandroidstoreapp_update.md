# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="e743e-101">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="e743e-101">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="e743e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e743e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e743e-103">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-103">Update the properties of a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e743e-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e743e-104">Prerequisites</span></span>
<span data-ttu-id="e743e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e743e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e743e-107">Permission type</span></span>|<span data-ttu-id="e743e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e743e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e743e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e743e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e743e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e743e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e743e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e743e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e743e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e743e-112">Not supported.</span></span>|
|<span data-ttu-id="e743e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e743e-113">Application</span></span>|<span data-ttu-id="e743e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e743e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e743e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e743e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e743e-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e743e-116">Request headers</span></span>
|<span data-ttu-id="e743e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e743e-117">Header</span></span>|<span data-ttu-id="e743e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e743e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e743e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e743e-119">Authorization</span></span>|<span data-ttu-id="e743e-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e743e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e743e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e743e-121">Accept</span></span>|<span data-ttu-id="e743e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e743e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e743e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e743e-123">Request body</span></span>
<span data-ttu-id="e743e-124">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e743e-124">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="e743e-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-125">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="e743e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e743e-126">Property</span></span>|<span data-ttu-id="e743e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e743e-127">Type</span></span>|<span data-ttu-id="e743e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e743e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e743e-129">id</span><span class="sxs-lookup"><span data-stu-id="e743e-129">id</span></span>|<span data-ttu-id="e743e-130">String</span><span class="sxs-lookup"><span data-stu-id="e743e-130">String</span></span>|<span data-ttu-id="e743e-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e743e-131">Key of the entity.</span></span> <span data-ttu-id="e743e-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e743e-133">displayName</span></span>|<span data-ttu-id="e743e-134">String</span><span class="sxs-lookup"><span data-stu-id="e743e-134">String</span></span>|<span data-ttu-id="e743e-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e743e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e743e-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-137">description</span><span class="sxs-lookup"><span data-stu-id="e743e-137">description</span></span>|<span data-ttu-id="e743e-138">String</span><span class="sxs-lookup"><span data-stu-id="e743e-138">String</span></span>|<span data-ttu-id="e743e-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-139">The description of the app.</span></span> <span data-ttu-id="e743e-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-141">publisher</span><span class="sxs-lookup"><span data-stu-id="e743e-141">publisher</span></span>|<span data-ttu-id="e743e-142">String</span><span class="sxs-lookup"><span data-stu-id="e743e-142">String</span></span>|<span data-ttu-id="e743e-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-143">The publisher of the app.</span></span> <span data-ttu-id="e743e-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e743e-145">largeIcon</span></span>|[<span data-ttu-id="e743e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e743e-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="e743e-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e743e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e743e-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e743e-149">createdDateTime</span></span>|<span data-ttu-id="e743e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e743e-150">DateTimeOffset</span></span>|<span data-ttu-id="e743e-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-151">The date and time the app was created.</span></span> <span data-ttu-id="e743e-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e743e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e743e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e743e-154">DateTimeOffset</span></span>|<span data-ttu-id="e743e-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-155">The date and time the app was last modified.</span></span> <span data-ttu-id="e743e-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e743e-157">isFeatured</span></span>|<span data-ttu-id="e743e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e743e-158">Boolean</span></span>|<span data-ttu-id="e743e-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e743e-160">privacyInformationUrl</span></span>|<span data-ttu-id="e743e-161">String</span><span class="sxs-lookup"><span data-stu-id="e743e-161">String</span></span>|<span data-ttu-id="e743e-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e743e-162">The privacy statement Url.</span></span> <span data-ttu-id="e743e-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e743e-164">informationUrl</span></span>|<span data-ttu-id="e743e-165">String</span><span class="sxs-lookup"><span data-stu-id="e743e-165">String</span></span>|<span data-ttu-id="e743e-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e743e-166">The more information Url.</span></span> <span data-ttu-id="e743e-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-168">owner</span><span class="sxs-lookup"><span data-stu-id="e743e-168">owner</span></span>|<span data-ttu-id="e743e-169">String</span><span class="sxs-lookup"><span data-stu-id="e743e-169">String</span></span>|<span data-ttu-id="e743e-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-170">The owner of the app.</span></span> <span data-ttu-id="e743e-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-172">developer</span><span class="sxs-lookup"><span data-stu-id="e743e-172">developer</span></span>|<span data-ttu-id="e743e-173">String</span><span class="sxs-lookup"><span data-stu-id="e743e-173">String</span></span>|<span data-ttu-id="e743e-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-174">The developer of the app.</span></span> <span data-ttu-id="e743e-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-176">notes</span><span class="sxs-lookup"><span data-stu-id="e743e-176">notes</span></span>|<span data-ttu-id="e743e-177">String</span><span class="sxs-lookup"><span data-stu-id="e743e-177">String</span></span>|<span data-ttu-id="e743e-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e743e-178">Notes for the app.</span></span> <span data-ttu-id="e743e-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e743e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="e743e-180">publishingState</span></span>|[<span data-ttu-id="e743e-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e743e-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="e743e-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-182">The publishing state for the app.</span></span> <span data-ttu-id="e743e-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e743e-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e743e-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="e743e-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e743e-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e743e-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e743e-186">appAvailability</span></span>|[<span data-ttu-id="e743e-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e743e-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="e743e-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-188">The Application's availability.</span></span> <span data-ttu-id="e743e-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="e743e-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e743e-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e743e-191">version</span><span class="sxs-lookup"><span data-stu-id="e743e-191">version</span></span>|<span data-ttu-id="e743e-192">String</span><span class="sxs-lookup"><span data-stu-id="e743e-192">String</span></span>|<span data-ttu-id="e743e-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-193">The Application's version.</span></span> <span data-ttu-id="e743e-194">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e743e-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="e743e-195">packageId</span><span class="sxs-lookup"><span data-stu-id="e743e-195">packageId</span></span>|<span data-ttu-id="e743e-196">String</span><span class="sxs-lookup"><span data-stu-id="e743e-196">String</span></span>|<span data-ttu-id="e743e-197">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="e743e-197">The app's package ID.</span></span>|
|<span data-ttu-id="e743e-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e743e-198">appStoreUrl</span></span>|<span data-ttu-id="e743e-199">String</span><span class="sxs-lookup"><span data-stu-id="e743e-199">String</span></span>|<span data-ttu-id="e743e-200">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="e743e-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="e743e-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e743e-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e743e-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e743e-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="e743e-203">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e743e-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e743e-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="e743e-204">Response</span></span>
<span data-ttu-id="e743e-205">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e743e-205">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e743e-206">Пример</span><span class="sxs-lookup"><span data-stu-id="e743e-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="e743e-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="e743e-207">Request</span></span>
<span data-ttu-id="e743e-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e743e-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

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

### <a name="response"></a><span data-ttu-id="e743e-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="e743e-209">Response</span></span>
<span data-ttu-id="e743e-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e743e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



