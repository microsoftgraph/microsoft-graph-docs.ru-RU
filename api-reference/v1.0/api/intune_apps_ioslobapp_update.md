# <a name="update-ioslobapp"></a><span data-ttu-id="55888-101">Обновление iosLobApp</span><span class="sxs-lookup"><span data-stu-id="55888-101">Update iosLobApp</span></span>

> <span data-ttu-id="55888-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55888-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55888-103">Обновление свойств объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-103">Update the properties of a [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55888-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="55888-104">Prerequisites</span></span>
<span data-ttu-id="55888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55888-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55888-107">Permission type</span></span>|<span data-ttu-id="55888-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55888-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55888-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55888-109">Delegated (work or school account)</span></span>|<span data-ttu-id="55888-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55888-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55888-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55888-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55888-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55888-112">Not supported.</span></span>|
|<span data-ttu-id="55888-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55888-113">Application</span></span>|<span data-ttu-id="55888-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55888-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55888-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55888-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="55888-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55888-116">Request headers</span></span>
|<span data-ttu-id="55888-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55888-117">Header</span></span>|<span data-ttu-id="55888-118">Значение</span><span class="sxs-lookup"><span data-stu-id="55888-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55888-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55888-119">Authorization</span></span>|<span data-ttu-id="55888-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="55888-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55888-121">Accept</span><span class="sxs-lookup"><span data-stu-id="55888-121">Accept</span></span>|<span data-ttu-id="55888-122">application/json</span><span class="sxs-lookup"><span data-stu-id="55888-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55888-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55888-123">Request body</span></span>
<span data-ttu-id="55888-124">В теле запроса добавьте представление объекта [iosLobApp](../resources/intune_apps_ioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55888-124">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="55888-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-125">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune_apps_ioslobapp.md).</span></span>

|<span data-ttu-id="55888-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="55888-126">Property</span></span>|<span data-ttu-id="55888-127">Тип</span><span class="sxs-lookup"><span data-stu-id="55888-127">Type</span></span>|<span data-ttu-id="55888-128">Описание</span><span class="sxs-lookup"><span data-stu-id="55888-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55888-129">id</span><span class="sxs-lookup"><span data-stu-id="55888-129">id</span></span>|<span data-ttu-id="55888-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-130">String</span></span>|<span data-ttu-id="55888-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55888-131">Key of the entity.</span></span> <span data-ttu-id="55888-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-133">displayName</span><span class="sxs-lookup"><span data-stu-id="55888-133">displayName</span></span>|<span data-ttu-id="55888-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-134">String</span></span>|<span data-ttu-id="55888-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="55888-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="55888-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-137">описание</span><span class="sxs-lookup"><span data-stu-id="55888-137">description</span></span>|<span data-ttu-id="55888-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-138">String</span></span>|<span data-ttu-id="55888-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-139">The description of the app.</span></span> <span data-ttu-id="55888-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-141">publisher</span><span class="sxs-lookup"><span data-stu-id="55888-141">publisher</span></span>|<span data-ttu-id="55888-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-142">String</span></span>|<span data-ttu-id="55888-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-143">The publisher of the app.</span></span> <span data-ttu-id="55888-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="55888-145">largeIcon</span></span>|[<span data-ttu-id="55888-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="55888-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="55888-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="55888-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="55888-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55888-149">createdDateTime</span></span>|<span data-ttu-id="55888-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55888-150">DateTimeOffset</span></span>|<span data-ttu-id="55888-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-151">The date and time the app was created.</span></span> <span data-ttu-id="55888-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55888-153">lastModifiedDateTime</span></span>|<span data-ttu-id="55888-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55888-154">DateTimeOffset</span></span>|<span data-ttu-id="55888-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-155">The date and time the app was last modified.</span></span> <span data-ttu-id="55888-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="55888-157">isFeatured</span></span>|<span data-ttu-id="55888-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="55888-158">Boolean</span></span>|<span data-ttu-id="55888-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="55888-160">privacyInformationUrl</span></span>|<span data-ttu-id="55888-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-161">String</span></span>|<span data-ttu-id="55888-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="55888-162">The privacy statement Url.</span></span> <span data-ttu-id="55888-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="55888-164">informationUrl</span></span>|<span data-ttu-id="55888-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-165">String</span></span>|<span data-ttu-id="55888-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="55888-166">The more information Url.</span></span> <span data-ttu-id="55888-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-168">owner</span><span class="sxs-lookup"><span data-stu-id="55888-168">owner</span></span>|<span data-ttu-id="55888-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-169">String</span></span>|<span data-ttu-id="55888-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-170">The owner of the app.</span></span> <span data-ttu-id="55888-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-172">developer</span><span class="sxs-lookup"><span data-stu-id="55888-172">developer</span></span>|<span data-ttu-id="55888-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-173">String</span></span>|<span data-ttu-id="55888-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-174">The developer of the app.</span></span> <span data-ttu-id="55888-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-176">notes</span><span class="sxs-lookup"><span data-stu-id="55888-176">notes</span></span>|<span data-ttu-id="55888-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-177">String</span></span>|<span data-ttu-id="55888-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="55888-178">Notes for the app.</span></span> <span data-ttu-id="55888-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55888-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="55888-180">publishingState</span></span>|[<span data-ttu-id="55888-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="55888-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="55888-p114">Состояние публикации для приложения. Приложение может быть назначено только в случае публикации приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="55888-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="55888-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="55888-186">committedContentVersion</span></span>|<span data-ttu-id="55888-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-187">String</span></span>|<span data-ttu-id="55888-188">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="55888-188">The internal committed content version.</span></span> <span data-ttu-id="55888-189">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55888-190">fileName</span><span class="sxs-lookup"><span data-stu-id="55888-190">fileName</span></span>|<span data-ttu-id="55888-191">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-191">String</span></span>|<span data-ttu-id="55888-192">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="55888-192">The name of the main Lob application file.</span></span> <span data-ttu-id="55888-193">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55888-194">size</span><span class="sxs-lookup"><span data-stu-id="55888-194">size</span></span>|<span data-ttu-id="55888-195">Int64</span><span class="sxs-lookup"><span data-stu-id="55888-195">Int64</span></span>|<span data-ttu-id="55888-196">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="55888-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="55888-197">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55888-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55888-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="55888-198">bundleId</span></span>|<span data-ttu-id="55888-199">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-199">String</span></span>|<span data-ttu-id="55888-200">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="55888-200">The Identity Name.</span></span>|
|<span data-ttu-id="55888-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="55888-201">applicableDeviceType</span></span>|[<span data-ttu-id="55888-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="55888-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="55888-203">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="55888-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="55888-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55888-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="55888-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55888-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="55888-206">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="55888-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="55888-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="55888-207">expirationDateTime</span></span>|<span data-ttu-id="55888-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55888-208">DateTimeOffset</span></span>|<span data-ttu-id="55888-209">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="55888-209">The expiration time.</span></span>|
|<span data-ttu-id="55888-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="55888-210">versionNumber</span></span>|<span data-ttu-id="55888-211">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-211">String</span></span>|<span data-ttu-id="55888-212">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="55888-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="55888-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="55888-213">buildNumber</span></span>|<span data-ttu-id="55888-214">String (строка)</span><span class="sxs-lookup"><span data-stu-id="55888-214">String</span></span>|<span data-ttu-id="55888-215">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="55888-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="55888-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="55888-216">Response</span></span>
<span data-ttu-id="55888-217">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosLobApp](../resources/intune_apps_ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="55888-217">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55888-218">Пример</span><span class="sxs-lookup"><span data-stu-id="55888-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="55888-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="55888-219">Request</span></span>
<span data-ttu-id="55888-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55888-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1205

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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="55888-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="55888-221">Response</span></span>
<span data-ttu-id="55888-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55888-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```








