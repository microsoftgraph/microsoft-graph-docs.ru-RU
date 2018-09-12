# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="19a3a-101">Создание managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="19a3a-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="19a3a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19a3a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19a3a-103">Создание нового объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-103">Create a new [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19a3a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="19a3a-104">Prerequisites</span></span>
<span data-ttu-id="19a3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19a3a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19a3a-107">Permission type</span></span>|<span data-ttu-id="19a3a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19a3a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19a3a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19a3a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="19a3a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a3a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19a3a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19a3a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19a3a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a3a-112">Not supported.</span></span>|
|<span data-ttu-id="19a3a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19a3a-113">Application</span></span>|<span data-ttu-id="19a3a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a3a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19a3a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19a3a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="19a3a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19a3a-116">Request headers</span></span>
|<span data-ttu-id="19a3a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19a3a-117">Header</span></span>|<span data-ttu-id="19a3a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="19a3a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19a3a-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19a3a-119">Authorization</span></span>|<span data-ttu-id="19a3a-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="19a3a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19a3a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="19a3a-121">Accept</span></span>|<span data-ttu-id="19a3a-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="19a3a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19a3a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19a3a-123">Request body</span></span>
<span data-ttu-id="19a3a-124">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19a3a-124">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="19a3a-125">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="19a3a-125">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="19a3a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="19a3a-126">Property</span></span>|<span data-ttu-id="19a3a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="19a3a-127">Type</span></span>|<span data-ttu-id="19a3a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="19a3a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a3a-129">id</span><span class="sxs-lookup"><span data-stu-id="19a3a-129">id</span></span>|<span data-ttu-id="19a3a-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-130">String</span></span>|<span data-ttu-id="19a3a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19a3a-131">Key of the entity.</span></span> <span data-ttu-id="19a3a-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="19a3a-133">displayName</span></span>|<span data-ttu-id="19a3a-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-134">String</span></span>|<span data-ttu-id="19a3a-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="19a3a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="19a3a-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-137">description</span><span class="sxs-lookup"><span data-stu-id="19a3a-137">description</span></span>|<span data-ttu-id="19a3a-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-138">String</span></span>|<span data-ttu-id="19a3a-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-139">The description of the app.</span></span> <span data-ttu-id="19a3a-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-141">издатель</span><span class="sxs-lookup"><span data-stu-id="19a3a-141">publisher</span></span>|<span data-ttu-id="19a3a-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-142">String</span></span>|<span data-ttu-id="19a3a-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-143">The publisher of the app.</span></span> <span data-ttu-id="19a3a-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="19a3a-145">largeIcon</span></span>|[<span data-ttu-id="19a3a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="19a3a-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="19a3a-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="19a3a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="19a3a-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19a3a-149">createdDateTime</span></span>|<span data-ttu-id="19a3a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a3a-150">DateTimeOffset</span></span>|<span data-ttu-id="19a3a-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-151">The date and time the app was created.</span></span> <span data-ttu-id="19a3a-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19a3a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="19a3a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a3a-154">DateTimeOffset</span></span>|<span data-ttu-id="19a3a-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-155">The date and time the app was last modified.</span></span> <span data-ttu-id="19a3a-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="19a3a-157">isFeatured</span></span>|<span data-ttu-id="19a3a-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="19a3a-158">Boolean</span></span>|<span data-ttu-id="19a3a-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="19a3a-160">privacyInformationUrl</span></span>|<span data-ttu-id="19a3a-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-161">String</span></span>|<span data-ttu-id="19a3a-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="19a3a-162">The privacy statement Url.</span></span> <span data-ttu-id="19a3a-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="19a3a-164">informationUrl</span></span>|<span data-ttu-id="19a3a-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-165">String</span></span>|<span data-ttu-id="19a3a-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="19a3a-166">The more information Url.</span></span> <span data-ttu-id="19a3a-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-168">ответственный</span><span class="sxs-lookup"><span data-stu-id="19a3a-168">owner</span></span>|<span data-ttu-id="19a3a-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-169">String</span></span>|<span data-ttu-id="19a3a-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-170">The owner of the app.</span></span> <span data-ttu-id="19a3a-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-172">разработчик</span><span class="sxs-lookup"><span data-stu-id="19a3a-172">developer</span></span>|<span data-ttu-id="19a3a-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-173">String</span></span>|<span data-ttu-id="19a3a-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-174">The developer of the app.</span></span> <span data-ttu-id="19a3a-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-176">заметки</span><span class="sxs-lookup"><span data-stu-id="19a3a-176">notes</span></span>|<span data-ttu-id="19a3a-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-177">String</span></span>|<span data-ttu-id="19a3a-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="19a3a-178">Notes for the app.</span></span> <span data-ttu-id="19a3a-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="19a3a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="19a3a-180">publishingState</span></span>|[<span data-ttu-id="19a3a-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="19a3a-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="19a3a-p114">Состояние публикации для приложения. Приложение может быть назначено только в случае публикации приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="19a3a-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="19a3a-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="19a3a-186">appAvailability</span></span>|[<span data-ttu-id="19a3a-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="19a3a-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="19a3a-p115">Доступность приложения. Наследуется от [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="19a3a-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="19a3a-191">version</span><span class="sxs-lookup"><span data-stu-id="19a3a-191">version</span></span>|<span data-ttu-id="19a3a-192">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-192">String</span></span>|<span data-ttu-id="19a3a-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-193">The Application's version.</span></span> <span data-ttu-id="19a3a-194">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="19a3a-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="19a3a-195">packageId</span><span class="sxs-lookup"><span data-stu-id="19a3a-195">packageId</span></span>|<span data-ttu-id="19a3a-196">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-196">String</span></span>|<span data-ttu-id="19a3a-197">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="19a3a-197">The app's package ID.</span></span>|
|<span data-ttu-id="19a3a-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="19a3a-198">appStoreUrl</span></span>|<span data-ttu-id="19a3a-199">String (строка)</span><span class="sxs-lookup"><span data-stu-id="19a3a-199">String</span></span>|<span data-ttu-id="19a3a-200">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="19a3a-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="19a3a-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="19a3a-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="19a3a-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="19a3a-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="19a3a-203">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="19a3a-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="19a3a-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="19a3a-204">Response</span></span>
<span data-ttu-id="19a3a-205">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19a3a-205">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a3a-206">Пример</span><span class="sxs-lookup"><span data-stu-id="19a3a-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="19a3a-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="19a3a-207">Request</span></span>
<span data-ttu-id="19a3a-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19a3a-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19a3a-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="19a3a-209">Response</span></span>
<span data-ttu-id="19a3a-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19a3a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








