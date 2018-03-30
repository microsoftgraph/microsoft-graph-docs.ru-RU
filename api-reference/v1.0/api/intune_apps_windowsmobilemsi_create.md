# <a name="create-windowsmobilemsi"></a><span data-ttu-id="0a6f5-101">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="0a6f5-101">Create windowsMobileMSI</span></span>

> <span data-ttu-id="0a6f5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a6f5-103">Создание объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-103">Create a new [plannerBucket](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a6f5-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0a6f5-104">Prerequisites</span></span>
<span data-ttu-id="0a6f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a6f5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a6f5-107">Permission type</span></span>|<span data-ttu-id="0a6f5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a6f5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a6f5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a6f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0a6f5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a6f5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a6f5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a6f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a6f5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-112">Not supported.</span></span>|
|<span data-ttu-id="0a6f5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a6f5-113">Application</span></span>|<span data-ttu-id="0a6f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a6f5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a6f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0a6f5-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a6f5-116">Request headers</span></span>
|<span data-ttu-id="0a6f5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a6f5-117">Header</span></span>|<span data-ttu-id="0a6f5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0a6f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a6f5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a6f5-119">Authorization</span></span>|<span data-ttu-id="0a6f5-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a6f5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0a6f5-121">Accept</span></span>|<span data-ttu-id="0a6f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0a6f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a6f5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a6f5-123">Request body</span></span>
<span data-ttu-id="0a6f5-124">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="0a6f5-125">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0a6f5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a6f5-126">Property</span></span>|<span data-ttu-id="0a6f5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0a6f5-127">Type</span></span>|<span data-ttu-id="0a6f5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0a6f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a6f5-129">id</span><span class="sxs-lookup"><span data-stu-id="0a6f5-129">id</span></span>|<span data-ttu-id="0a6f5-130">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-130">String</span></span>|<span data-ttu-id="0a6f5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-131">Key of the setting.</span></span> <span data-ttu-id="0a6f5-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0a6f5-133">displayName</span></span>|<span data-ttu-id="0a6f5-134">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-134">String</span></span>|<span data-ttu-id="0a6f5-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0a6f5-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-137">description</span><span class="sxs-lookup"><span data-stu-id="0a6f5-137">description</span></span>|<span data-ttu-id="0a6f5-138">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-138">String</span></span>|<span data-ttu-id="0a6f5-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-139">The description of the app.</span></span> <span data-ttu-id="0a6f5-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-141">publisher</span><span class="sxs-lookup"><span data-stu-id="0a6f5-141">Publisher</span></span>|<span data-ttu-id="0a6f5-142">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-142">String</span></span>|<span data-ttu-id="0a6f5-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-143">The name of the app.</span></span> <span data-ttu-id="0a6f5-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0a6f5-145">largeIcon</span></span>|[<span data-ttu-id="0a6f5-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a6f5-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="0a6f5-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0a6f5-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a6f5-149">createdDateTime</span></span>|<span data-ttu-id="0a6f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a6f5-150">DateTimeOffset</span></span>|<span data-ttu-id="0a6f5-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-151">The date and time the group was created.</span></span> <span data-ttu-id="0a6f5-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a6f5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0a6f5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a6f5-154">DateTimeOffset</span></span>|<span data-ttu-id="0a6f5-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="0a6f5-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0a6f5-157">isFeatured</span></span>|<span data-ttu-id="0a6f5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a6f5-158">Boolean</span></span>|<span data-ttu-id="0a6f5-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0a6f5-160">privacyInformationUrl</span></span>|<span data-ttu-id="0a6f5-161">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-161">String</span></span>|<span data-ttu-id="0a6f5-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-162">The privacy statement Url.</span></span> <span data-ttu-id="0a6f5-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0a6f5-164">informationUrl</span></span>|<span data-ttu-id="0a6f5-165">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-165">String</span></span>|<span data-ttu-id="0a6f5-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-166">The more information Url.</span></span> <span data-ttu-id="0a6f5-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-168">owner</span><span class="sxs-lookup"><span data-stu-id="0a6f5-168">owner</span></span>|<span data-ttu-id="0a6f5-169">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-169">String</span></span>|<span data-ttu-id="0a6f5-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-170">The owner of the app.</span></span> <span data-ttu-id="0a6f5-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-172">developer</span><span class="sxs-lookup"><span data-stu-id="0a6f5-172">developer</span></span>|<span data-ttu-id="0a6f5-173">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-173">String</span></span>|<span data-ttu-id="0a6f5-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-174">The name of the app.</span></span> <span data-ttu-id="0a6f5-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-176">notes</span><span class="sxs-lookup"><span data-stu-id="0a6f5-176">Notes</span></span>|<span data-ttu-id="0a6f5-177">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-177">String</span></span>|<span data-ttu-id="0a6f5-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-178">Notes for the app.</span></span> <span data-ttu-id="0a6f5-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0a6f5-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0a6f5-180">publishingState</span></span>|<span data-ttu-id="0a6f5-181">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-181">String</span></span>|<span data-ttu-id="0a6f5-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-182">The publishing state for the app.</span></span> <span data-ttu-id="0a6f5-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0a6f5-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0a6f5-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0a6f5-185">committedContentVersion</span></span>|<span data-ttu-id="0a6f5-186">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-186">String</span></span>|<span data-ttu-id="0a6f5-187">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-187">The internal committed content version.</span></span> <span data-ttu-id="0a6f5-188">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0a6f5-189">fileName</span><span class="sxs-lookup"><span data-stu-id="0a6f5-189">fileName</span></span>|<span data-ttu-id="0a6f5-190">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-190">String</span></span>|<span data-ttu-id="0a6f5-191">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-191">The name of the main Lob application file.</span></span> <span data-ttu-id="0a6f5-192">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0a6f5-193">size</span><span class="sxs-lookup"><span data-stu-id="0a6f5-193">size</span></span>|<span data-ttu-id="0a6f5-194">Int64</span><span class="sxs-lookup"><span data-stu-id="0a6f5-194">Int64</span></span>|<span data-ttu-id="0a6f5-195">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="0a6f5-196">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0a6f5-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0a6f5-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="0a6f5-197">Command-line:</span></span>|<span data-ttu-id="0a6f5-198">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-198">String</span></span>|<span data-ttu-id="0a6f5-199">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-199">The command line.</span></span>|
|<span data-ttu-id="0a6f5-200">productCode</span><span class="sxs-lookup"><span data-stu-id="0a6f5-200">productCode</span></span>|<span data-ttu-id="0a6f5-201">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-201">String</span></span>|<span data-ttu-id="0a6f5-202">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-202">The product code.</span></span>|
|<span data-ttu-id="0a6f5-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="0a6f5-203">productVersion</span></span>|<span data-ttu-id="0a6f5-204">String</span><span class="sxs-lookup"><span data-stu-id="0a6f5-204">String</span></span>|<span data-ttu-id="0a6f5-205">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0a6f5-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="0a6f5-206">ignoreVersionDetection</span></span>|<span data-ttu-id="0a6f5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a6f5-207">Boolean</span></span>|<span data-ttu-id="0a6f5-208">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="0a6f5-209">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="0a6f5-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a6f5-210">Response</span></span>
<span data-ttu-id="0a6f5-211">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-211">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a6f5-212">Пример</span><span class="sxs-lookup"><span data-stu-id="0a6f5-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a6f5-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a6f5-213">Request</span></span>
<span data-ttu-id="0a6f5-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a6f5-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a6f5-215">Response</span></span>
<span data-ttu-id="0a6f5-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0a6f5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



