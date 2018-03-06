# <a name="update-windowsmobilemsi"></a><span data-ttu-id="133ca-101">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="133ca-101">Update windowsMobileMSI</span></span>

> <span data-ttu-id="133ca-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="133ca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="133ca-103">Обновление свойств объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-103">Update the properties of a [calendar](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="133ca-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="133ca-104">Prerequisites</span></span>
<span data-ttu-id="133ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="133ca-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="133ca-107">Permission type</span></span>|<span data-ttu-id="133ca-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="133ca-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="133ca-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="133ca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="133ca-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="133ca-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="133ca-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="133ca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="133ca-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="133ca-112">Not supported.</span></span>|
|<span data-ttu-id="133ca-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="133ca-113">Application</span></span>|<span data-ttu-id="133ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="133ca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="133ca-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="133ca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="133ca-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="133ca-116">Request headers</span></span>
|<span data-ttu-id="133ca-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="133ca-117">Header</span></span>|<span data-ttu-id="133ca-118">Значение</span><span class="sxs-lookup"><span data-stu-id="133ca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="133ca-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="133ca-119">Authorization</span></span>|<span data-ttu-id="133ca-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="133ca-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="133ca-121">Accept</span><span class="sxs-lookup"><span data-stu-id="133ca-121">Accept</span></span>|<span data-ttu-id="133ca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="133ca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="133ca-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="133ca-123">Request body</span></span>
<span data-ttu-id="133ca-124">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="133ca-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="133ca-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="133ca-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="133ca-126">Property</span></span>|<span data-ttu-id="133ca-127">Тип</span><span class="sxs-lookup"><span data-stu-id="133ca-127">Type</span></span>|<span data-ttu-id="133ca-128">Описание</span><span class="sxs-lookup"><span data-stu-id="133ca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="133ca-129">id</span><span class="sxs-lookup"><span data-stu-id="133ca-129">id</span></span>|<span data-ttu-id="133ca-130">String</span><span class="sxs-lookup"><span data-stu-id="133ca-130">String</span></span>|<span data-ttu-id="133ca-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="133ca-131">Key of the setting.</span></span> <span data-ttu-id="133ca-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-133">displayName</span><span class="sxs-lookup"><span data-stu-id="133ca-133">displayName</span></span>|<span data-ttu-id="133ca-134">String</span><span class="sxs-lookup"><span data-stu-id="133ca-134">String</span></span>|<span data-ttu-id="133ca-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="133ca-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="133ca-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-137">description</span><span class="sxs-lookup"><span data-stu-id="133ca-137">description</span></span>|<span data-ttu-id="133ca-138">String</span><span class="sxs-lookup"><span data-stu-id="133ca-138">String</span></span>|<span data-ttu-id="133ca-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-139">The description of the app.</span></span> <span data-ttu-id="133ca-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-141">publisher</span><span class="sxs-lookup"><span data-stu-id="133ca-141">Publisher</span></span>|<span data-ttu-id="133ca-142">String</span><span class="sxs-lookup"><span data-stu-id="133ca-142">String</span></span>|<span data-ttu-id="133ca-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-143">The name of the app.</span></span> <span data-ttu-id="133ca-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="133ca-145">largeIcon</span></span>|[<span data-ttu-id="133ca-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="133ca-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="133ca-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="133ca-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="133ca-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="133ca-149">createdDateTime</span></span>|<span data-ttu-id="133ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133ca-150">DateTimeOffset</span></span>|<span data-ttu-id="133ca-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-151">The date and time the group was created.</span></span> <span data-ttu-id="133ca-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="133ca-153">lastModifiedDateTime</span></span>|<span data-ttu-id="133ca-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133ca-154">DateTimeOffset</span></span>|<span data-ttu-id="133ca-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="133ca-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="133ca-157">isFeatured</span></span>|<span data-ttu-id="133ca-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="133ca-158">Boolean</span></span>|<span data-ttu-id="133ca-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="133ca-160">privacyInformationUrl</span></span>|<span data-ttu-id="133ca-161">String</span><span class="sxs-lookup"><span data-stu-id="133ca-161">String</span></span>|<span data-ttu-id="133ca-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="133ca-162">The privacy statement Url.</span></span> <span data-ttu-id="133ca-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="133ca-164">informationUrl</span></span>|<span data-ttu-id="133ca-165">String</span><span class="sxs-lookup"><span data-stu-id="133ca-165">String</span></span>|<span data-ttu-id="133ca-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="133ca-166">The more information Url.</span></span> <span data-ttu-id="133ca-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-168">owner</span><span class="sxs-lookup"><span data-stu-id="133ca-168">owner</span></span>|<span data-ttu-id="133ca-169">String</span><span class="sxs-lookup"><span data-stu-id="133ca-169">String</span></span>|<span data-ttu-id="133ca-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-170">The owner of the app.</span></span> <span data-ttu-id="133ca-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-172">developer</span><span class="sxs-lookup"><span data-stu-id="133ca-172">developer</span></span>|<span data-ttu-id="133ca-173">String</span><span class="sxs-lookup"><span data-stu-id="133ca-173">String</span></span>|<span data-ttu-id="133ca-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-174">The name of the app.</span></span> <span data-ttu-id="133ca-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-176">notes</span><span class="sxs-lookup"><span data-stu-id="133ca-176">Notes</span></span>|<span data-ttu-id="133ca-177">String</span><span class="sxs-lookup"><span data-stu-id="133ca-177">String</span></span>|<span data-ttu-id="133ca-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-178">Notes for the app.</span></span> <span data-ttu-id="133ca-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133ca-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="133ca-180">publishingState</span></span>|<span data-ttu-id="133ca-181">String</span><span class="sxs-lookup"><span data-stu-id="133ca-181">String</span></span>|<span data-ttu-id="133ca-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-182">The publishing state for the app.</span></span> <span data-ttu-id="133ca-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="133ca-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="133ca-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="133ca-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="133ca-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="133ca-185">committedContentVersion</span></span>|<span data-ttu-id="133ca-186">String</span><span class="sxs-lookup"><span data-stu-id="133ca-186">String</span></span>|<span data-ttu-id="133ca-187">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="133ca-187">The internal committed content version.</span></span> <span data-ttu-id="133ca-188">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133ca-189">fileName</span><span class="sxs-lookup"><span data-stu-id="133ca-189">fileName</span></span>|<span data-ttu-id="133ca-190">String</span><span class="sxs-lookup"><span data-stu-id="133ca-190">String</span></span>|<span data-ttu-id="133ca-191">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="133ca-191">The name of the main Lob application file.</span></span> <span data-ttu-id="133ca-192">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133ca-193">size</span><span class="sxs-lookup"><span data-stu-id="133ca-193">size</span></span>|<span data-ttu-id="133ca-194">Int64</span><span class="sxs-lookup"><span data-stu-id="133ca-194">Int64</span></span>|<span data-ttu-id="133ca-195">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="133ca-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="133ca-196">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="133ca-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133ca-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="133ca-197">Command-line:</span></span>|<span data-ttu-id="133ca-198">String</span><span class="sxs-lookup"><span data-stu-id="133ca-198">String</span></span>|<span data-ttu-id="133ca-199">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="133ca-199">The command line.</span></span>|
|<span data-ttu-id="133ca-200">productCode</span><span class="sxs-lookup"><span data-stu-id="133ca-200">productCode</span></span>|<span data-ttu-id="133ca-201">String</span><span class="sxs-lookup"><span data-stu-id="133ca-201">String</span></span>|<span data-ttu-id="133ca-202">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="133ca-202">The product code.</span></span>|
|<span data-ttu-id="133ca-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="133ca-203">productVersion</span></span>|<span data-ttu-id="133ca-204">String</span><span class="sxs-lookup"><span data-stu-id="133ca-204">String</span></span>|<span data-ttu-id="133ca-205">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="133ca-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="133ca-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="133ca-206">ignoreVersionDetection</span></span>|<span data-ttu-id="133ca-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="133ca-207">Boolean</span></span>|<span data-ttu-id="133ca-208">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="133ca-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="133ca-209">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="133ca-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="133ca-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="133ca-210">Response</span></span>
<span data-ttu-id="133ca-211">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="133ca-211">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="133ca-212">Пример</span><span class="sxs-lookup"><span data-stu-id="133ca-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="133ca-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="133ca-213">Request</span></span>
<span data-ttu-id="133ca-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="133ca-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 864

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="133ca-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="133ca-215">Response</span></span>
<span data-ttu-id="133ca-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="133ca-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



