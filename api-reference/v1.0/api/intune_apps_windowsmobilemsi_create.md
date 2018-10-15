# <a name="create-windowsmobilemsi"></a><span data-ttu-id="d635e-101">Создание windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d635e-101">Create windowsMobileMSI</span></span>

> <span data-ttu-id="d635e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d635e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d635e-103">Создание объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-103">Create a new [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d635e-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d635e-104">Prerequisites</span></span>
<span data-ttu-id="d635e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d635e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d635e-107">Permission type</span></span>|<span data-ttu-id="d635e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d635e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d635e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d635e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d635e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d635e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d635e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d635e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d635e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d635e-112">Not supported.</span></span>|
|<span data-ttu-id="d635e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d635e-113">Application</span></span>|<span data-ttu-id="d635e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d635e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d635e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d635e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d635e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d635e-116">Request headers</span></span>
|<span data-ttu-id="d635e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d635e-117">Header</span></span>|<span data-ttu-id="d635e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d635e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d635e-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d635e-119">Authorization</span></span>|<span data-ttu-id="d635e-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="d635e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d635e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d635e-121">Accept</span></span>|<span data-ttu-id="d635e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d635e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d635e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d635e-123">Request body</span></span>
<span data-ttu-id="d635e-124">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d635e-124">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="d635e-125">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="d635e-125">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="d635e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d635e-126">Property</span></span>|<span data-ttu-id="d635e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d635e-127">Type</span></span>|<span data-ttu-id="d635e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d635e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d635e-129">id</span><span class="sxs-lookup"><span data-stu-id="d635e-129">id</span></span>|<span data-ttu-id="d635e-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-130">String</span></span>|<span data-ttu-id="d635e-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d635e-131">Key of the entity.</span></span> <span data-ttu-id="d635e-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d635e-133">displayName</span></span>|<span data-ttu-id="d635e-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-134">String</span></span>|<span data-ttu-id="d635e-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d635e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d635e-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-137">description</span><span class="sxs-lookup"><span data-stu-id="d635e-137">description</span></span>|<span data-ttu-id="d635e-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-138">String</span></span>|<span data-ttu-id="d635e-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-139">The description of the app.</span></span> <span data-ttu-id="d635e-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d635e-141">publisher</span></span>|<span data-ttu-id="d635e-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-142">String</span></span>|<span data-ttu-id="d635e-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-143">The publisher of the app.</span></span> <span data-ttu-id="d635e-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d635e-145">largeIcon</span></span>|[<span data-ttu-id="d635e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d635e-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="d635e-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d635e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d635e-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d635e-149">createdDateTime</span></span>|<span data-ttu-id="d635e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d635e-150">DateTimeOffset</span></span>|<span data-ttu-id="d635e-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-151">The date and time the app was created.</span></span> <span data-ttu-id="d635e-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d635e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d635e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d635e-154">DateTimeOffset</span></span>|<span data-ttu-id="d635e-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-155">The date and time the app was last modified.</span></span> <span data-ttu-id="d635e-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d635e-157">isFeatured</span></span>|<span data-ttu-id="d635e-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d635e-158">Boolean</span></span>|<span data-ttu-id="d635e-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d635e-160">privacyInformationUrl</span></span>|<span data-ttu-id="d635e-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-161">String</span></span>|<span data-ttu-id="d635e-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d635e-162">The privacy statement Url.</span></span> <span data-ttu-id="d635e-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d635e-164">informationUrl</span></span>|<span data-ttu-id="d635e-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-165">String</span></span>|<span data-ttu-id="d635e-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d635e-166">The more information Url.</span></span> <span data-ttu-id="d635e-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-168">owner</span><span class="sxs-lookup"><span data-stu-id="d635e-168">owner</span></span>|<span data-ttu-id="d635e-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-169">String</span></span>|<span data-ttu-id="d635e-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-170">The owner of the app.</span></span> <span data-ttu-id="d635e-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-172">developer</span><span class="sxs-lookup"><span data-stu-id="d635e-172">developer</span></span>|<span data-ttu-id="d635e-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-173">String</span></span>|<span data-ttu-id="d635e-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-174">The developer of the app.</span></span> <span data-ttu-id="d635e-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-176">notes</span><span class="sxs-lookup"><span data-stu-id="d635e-176">notes</span></span>|<span data-ttu-id="d635e-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-177">String</span></span>|<span data-ttu-id="d635e-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="d635e-178">Notes for the app.</span></span> <span data-ttu-id="d635e-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d635e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d635e-180">publishingState</span></span>|[<span data-ttu-id="d635e-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d635e-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="d635e-p114">Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d635e-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d635e-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d635e-186">committedContentVersion</span></span>|<span data-ttu-id="d635e-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-187">String</span></span>|<span data-ttu-id="d635e-188">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="d635e-188">The internal committed content version.</span></span> <span data-ttu-id="d635e-189">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d635e-190">fileName</span><span class="sxs-lookup"><span data-stu-id="d635e-190">fileName</span></span>|<span data-ttu-id="d635e-191">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-191">String</span></span>|<span data-ttu-id="d635e-192">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="d635e-192">The name of the main Lob application file.</span></span> <span data-ttu-id="d635e-193">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d635e-194">size</span><span class="sxs-lookup"><span data-stu-id="d635e-194">size</span></span>|<span data-ttu-id="d635e-195">Int64</span><span class="sxs-lookup"><span data-stu-id="d635e-195">Int64</span></span>|<span data-ttu-id="d635e-196">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="d635e-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="d635e-197">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d635e-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d635e-198">commandLine</span><span class="sxs-lookup"><span data-stu-id="d635e-198">commandLine</span></span>|<span data-ttu-id="d635e-199">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-199">String</span></span>|<span data-ttu-id="d635e-200">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="d635e-200">The command line.</span></span>|
|<span data-ttu-id="d635e-201">productCode</span><span class="sxs-lookup"><span data-stu-id="d635e-201">productCode</span></span>|<span data-ttu-id="d635e-202">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-202">String</span></span>|<span data-ttu-id="d635e-203">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="d635e-203">The product code.</span></span>|
|<span data-ttu-id="d635e-204">productVersion</span><span class="sxs-lookup"><span data-stu-id="d635e-204">productVersion</span></span>|<span data-ttu-id="d635e-205">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d635e-205">String</span></span>|<span data-ttu-id="d635e-206">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="d635e-206">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d635e-207">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d635e-207">ignoreVersionDetection</span></span>|<span data-ttu-id="d635e-208">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d635e-208">Boolean</span></span>|<span data-ttu-id="d635e-209">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d635e-209">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d635e-210">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="d635e-210">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="d635e-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="d635e-211">Response</span></span>
<span data-ttu-id="d635e-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d635e-212">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d635e-213">Пример</span><span class="sxs-lookup"><span data-stu-id="d635e-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="d635e-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="d635e-214">Request</span></span>
<span data-ttu-id="d635e-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d635e-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 919

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="d635e-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="d635e-216">Response</span></span>
<span data-ttu-id="d635e-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d635e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```








