# <a name="update-androidlobapp"></a><span data-ttu-id="328db-101">Обновление androidLobApp</span><span class="sxs-lookup"><span data-stu-id="328db-101">Update androidLobApp</span></span>

> <span data-ttu-id="328db-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="328db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="328db-103">Обновление свойств объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-103">Update the properties of a [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="328db-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="328db-104">Prerequisites</span></span>
<span data-ttu-id="328db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="328db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="328db-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="328db-107">Permission type</span></span>|<span data-ttu-id="328db-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="328db-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="328db-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="328db-109">Delegated (work or school account)</span></span>|<span data-ttu-id="328db-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="328db-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="328db-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="328db-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="328db-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="328db-112">Not supported.</span></span>|
|<span data-ttu-id="328db-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="328db-113">Application</span></span>|<span data-ttu-id="328db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="328db-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="328db-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="328db-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="328db-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="328db-116">Request headers</span></span>
|<span data-ttu-id="328db-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="328db-117">Header</span></span>|<span data-ttu-id="328db-118">Значение</span><span class="sxs-lookup"><span data-stu-id="328db-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="328db-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="328db-119">Authorization</span></span>|<span data-ttu-id="328db-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="328db-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="328db-121">Accept</span><span class="sxs-lookup"><span data-stu-id="328db-121">Accept</span></span>|<span data-ttu-id="328db-122">application/json</span><span class="sxs-lookup"><span data-stu-id="328db-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="328db-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="328db-123">Request body</span></span>
<span data-ttu-id="328db-124">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune_apps_androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="328db-124">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="328db-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-125">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune_apps_androidlobapp.md).</span></span>

|<span data-ttu-id="328db-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="328db-126">Property</span></span>|<span data-ttu-id="328db-127">Тип</span><span class="sxs-lookup"><span data-stu-id="328db-127">Type</span></span>|<span data-ttu-id="328db-128">Описание</span><span class="sxs-lookup"><span data-stu-id="328db-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="328db-129">id</span><span class="sxs-lookup"><span data-stu-id="328db-129">id</span></span>|<span data-ttu-id="328db-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-130">String</span></span>|<span data-ttu-id="328db-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="328db-131">Key of the entity.</span></span> <span data-ttu-id="328db-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-133">displayName</span><span class="sxs-lookup"><span data-stu-id="328db-133">displayName</span></span>|<span data-ttu-id="328db-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-134">String</span></span>|<span data-ttu-id="328db-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="328db-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="328db-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-137">description</span><span class="sxs-lookup"><span data-stu-id="328db-137">description</span></span>|<span data-ttu-id="328db-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-138">String</span></span>|<span data-ttu-id="328db-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-139">The description of the app.</span></span> <span data-ttu-id="328db-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-141">publisher</span><span class="sxs-lookup"><span data-stu-id="328db-141">publisher</span></span>|<span data-ttu-id="328db-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-142">String</span></span>|<span data-ttu-id="328db-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-143">The publisher of the app.</span></span> <span data-ttu-id="328db-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="328db-145">largeIcon</span></span>|[<span data-ttu-id="328db-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="328db-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="328db-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="328db-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="328db-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="328db-149">createdDateTime</span></span>|<span data-ttu-id="328db-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="328db-150">DateTimeOffset</span></span>|<span data-ttu-id="328db-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-151">The date and time the app was created.</span></span> <span data-ttu-id="328db-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="328db-153">lastModifiedDateTime</span></span>|<span data-ttu-id="328db-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="328db-154">DateTimeOffset</span></span>|<span data-ttu-id="328db-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-155">The date and time the app was last modified.</span></span> <span data-ttu-id="328db-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="328db-157">isFeatured</span></span>|<span data-ttu-id="328db-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="328db-158">Boolean</span></span>|<span data-ttu-id="328db-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="328db-160">privacyInformationUrl</span></span>|<span data-ttu-id="328db-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-161">String</span></span>|<span data-ttu-id="328db-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="328db-162">The privacy statement Url.</span></span> <span data-ttu-id="328db-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="328db-164">informationUrl</span></span>|<span data-ttu-id="328db-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-165">String</span></span>|<span data-ttu-id="328db-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="328db-166">The more information Url.</span></span> <span data-ttu-id="328db-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-168">owner</span><span class="sxs-lookup"><span data-stu-id="328db-168">owner</span></span>|<span data-ttu-id="328db-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-169">String</span></span>|<span data-ttu-id="328db-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-170">The owner of the app.</span></span> <span data-ttu-id="328db-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-172">developer</span><span class="sxs-lookup"><span data-stu-id="328db-172">developer</span></span>|<span data-ttu-id="328db-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-173">String</span></span>|<span data-ttu-id="328db-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-174">The developer of the app.</span></span> <span data-ttu-id="328db-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-176">notes</span><span class="sxs-lookup"><span data-stu-id="328db-176">notes</span></span>|<span data-ttu-id="328db-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-177">String</span></span>|<span data-ttu-id="328db-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="328db-178">Notes for the app.</span></span> <span data-ttu-id="328db-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="328db-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="328db-180">publishingState</span></span>|[<span data-ttu-id="328db-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="328db-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="328db-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-182">The publishing state for the app.</span></span> <span data-ttu-id="328db-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="328db-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="328db-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="328db-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="328db-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="328db-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="328db-186">committedContentVersion</span></span>|<span data-ttu-id="328db-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-187">String</span></span>|<span data-ttu-id="328db-188">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="328db-188">The internal committed content version.</span></span> <span data-ttu-id="328db-189">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="328db-190">fileName</span><span class="sxs-lookup"><span data-stu-id="328db-190">fileName</span></span>|<span data-ttu-id="328db-191">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-191">String</span></span>|<span data-ttu-id="328db-192">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="328db-192">The name of the main Lob application file.</span></span> <span data-ttu-id="328db-193">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="328db-194">size</span><span class="sxs-lookup"><span data-stu-id="328db-194">size</span></span>|<span data-ttu-id="328db-195">Int64</span><span class="sxs-lookup"><span data-stu-id="328db-195">Int64</span></span>|<span data-ttu-id="328db-196">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="328db-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="328db-197">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="328db-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="328db-198">packageId</span><span class="sxs-lookup"><span data-stu-id="328db-198">packageId</span></span>|<span data-ttu-id="328db-199">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-199">String</span></span>|<span data-ttu-id="328db-200">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="328db-200">The package identifier.</span></span>|
|<span data-ttu-id="328db-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="328db-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="328db-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="328db-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="328db-203">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="328db-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="328db-204">versionName</span><span class="sxs-lookup"><span data-stu-id="328db-204">versionName</span></span>|<span data-ttu-id="328db-205">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-205">String</span></span>|<span data-ttu-id="328db-206">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="328db-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="328db-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="328db-207">versionCode</span></span>|<span data-ttu-id="328db-208">String (строка)</span><span class="sxs-lookup"><span data-stu-id="328db-208">String</span></span>|<span data-ttu-id="328db-209">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="328db-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="328db-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="328db-210">Response</span></span>
<span data-ttu-id="328db-211">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune_apps_androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="328db-211">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="328db-212">Пример</span><span class="sxs-lookup"><span data-stu-id="328db-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="328db-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="328db-213">Request</span></span>
<span data-ttu-id="328db-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="328db-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="328db-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="328db-215">Response</span></span>
<span data-ttu-id="328db-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="328db-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



