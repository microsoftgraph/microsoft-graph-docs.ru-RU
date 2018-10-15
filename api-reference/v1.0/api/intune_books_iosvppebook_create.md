# <a name="create-iosvppebook"></a><span data-ttu-id="fdda1-101">Создание iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="fdda1-101">Create iosVppEBook</span></span>

> <span data-ttu-id="fdda1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdda1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdda1-103">Создание объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-103">Create a new [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdda1-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fdda1-104">Prerequisites</span></span>
<span data-ttu-id="fdda1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdda1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdda1-107">Permission type</span></span>|<span data-ttu-id="fdda1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdda1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdda1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdda1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fdda1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdda1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fdda1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdda1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdda1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdda1-112">Not supported.</span></span>|
|<span data-ttu-id="fdda1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdda1-113">Application</span></span>|<span data-ttu-id="fdda1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdda1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdda1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdda1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="fdda1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdda1-116">Request headers</span></span>
|<span data-ttu-id="fdda1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdda1-117">Header</span></span>|<span data-ttu-id="fdda1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fdda1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdda1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdda1-119">Authorization</span></span>|<span data-ttu-id="fdda1-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fdda1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdda1-121">Принять</span><span class="sxs-lookup"><span data-stu-id="fdda1-121">Accept</span></span>|<span data-ttu-id="fdda1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fdda1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdda1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdda1-123">Request body</span></span>
<span data-ttu-id="fdda1-124">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdda1-124">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="fdda1-125">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="fdda1-125">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="fdda1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdda1-126">Property</span></span>|<span data-ttu-id="fdda1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fdda1-127">Type</span></span>|<span data-ttu-id="fdda1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fdda1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdda1-129">ид</span><span class="sxs-lookup"><span data-stu-id="fdda1-129">id</span></span>|<span data-ttu-id="fdda1-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-130">String</span></span>|<span data-ttu-id="fdda1-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdda1-131">Key of the entity.</span></span> <span data-ttu-id="fdda1-132">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fdda1-133">displayName</span></span>|<span data-ttu-id="fdda1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-134">String</span></span>|<span data-ttu-id="fdda1-135">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fdda1-135">Name of the eBook.</span></span> <span data-ttu-id="fdda1-136">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-137">описание</span><span class="sxs-lookup"><span data-stu-id="fdda1-137">description</span></span>|<span data-ttu-id="fdda1-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-138">String</span></span>|<span data-ttu-id="fdda1-139">Описание.</span><span class="sxs-lookup"><span data-stu-id="fdda1-139">Description.</span></span> <span data-ttu-id="fdda1-140">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-141">издатель</span><span class="sxs-lookup"><span data-stu-id="fdda1-141">publisher</span></span>|<span data-ttu-id="fdda1-142">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-142">String</span></span>|<span data-ttu-id="fdda1-143">Издатель.</span><span class="sxs-lookup"><span data-stu-id="fdda1-143">Publisher.</span></span> <span data-ttu-id="fdda1-144">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdda1-145">publishedDateTime</span></span>|<span data-ttu-id="fdda1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdda1-146">DateTimeOffset</span></span>|<span data-ttu-id="fdda1-147">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fdda1-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="fdda1-148">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="fdda1-149">largeCover</span></span>|[<span data-ttu-id="fdda1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fdda1-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="fdda1-151">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="fdda1-151">Book cover.</span></span> <span data-ttu-id="fdda1-152">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdda1-153">createdDateTime</span></span>|<span data-ttu-id="fdda1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdda1-154">DateTimeOffset</span></span>|<span data-ttu-id="fdda1-155">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fdda1-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="fdda1-156">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdda1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fdda1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdda1-158">DateTimeOffset</span></span>|<span data-ttu-id="fdda1-159">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fdda1-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="fdda1-160">Унаследован от объекта [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="fdda1-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fdda1-161">informationUrl</span></span>|<span data-ttu-id="fdda1-162">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-162">String</span></span>|<span data-ttu-id="fdda1-163">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fdda1-163">The more information Url.</span></span> <span data-ttu-id="fdda1-164">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fdda1-165">privacyInformationUrl</span></span>|<span data-ttu-id="fdda1-166">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-166">String</span></span>|<span data-ttu-id="fdda1-167">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fdda1-167">The privacy statement Url.</span></span> <span data-ttu-id="fdda1-168">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fdda1-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="fdda1-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="fdda1-169">vppTokenId</span></span>|<span data-ttu-id="fdda1-170">Guid</span><span class="sxs-lookup"><span data-stu-id="fdda1-170">Guid</span></span>|<span data-ttu-id="fdda1-171">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="fdda1-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="fdda1-172">appleId</span><span class="sxs-lookup"><span data-stu-id="fdda1-172">appleId</span></span>|<span data-ttu-id="fdda1-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-173">String</span></span>|<span data-ttu-id="fdda1-174">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="fdda1-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="fdda1-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="fdda1-175">vppOrganizationName</span></span>|<span data-ttu-id="fdda1-176">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-176">String</span></span>|<span data-ttu-id="fdda1-177">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="fdda1-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="fdda1-178">жанры</span><span class="sxs-lookup"><span data-stu-id="fdda1-178">genres</span></span>|<span data-ttu-id="fdda1-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fdda1-179">String collection</span></span>|<span data-ttu-id="fdda1-180">Жанры.</span><span class="sxs-lookup"><span data-stu-id="fdda1-180">Genres.</span></span>|
|<span data-ttu-id="fdda1-181">язык</span><span class="sxs-lookup"><span data-stu-id="fdda1-181">language</span></span>|<span data-ttu-id="fdda1-182">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-182">String</span></span>|<span data-ttu-id="fdda1-183">Язык.</span><span class="sxs-lookup"><span data-stu-id="fdda1-183">Language.</span></span>|
|<span data-ttu-id="fdda1-184">автор</span><span class="sxs-lookup"><span data-stu-id="fdda1-184">seller</span></span>|<span data-ttu-id="fdda1-185">Строка</span><span class="sxs-lookup"><span data-stu-id="fdda1-185">String</span></span>|<span data-ttu-id="fdda1-186">Продавец.</span><span class="sxs-lookup"><span data-stu-id="fdda1-186">Seller.</span></span>|
|<span data-ttu-id="fdda1-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="fdda1-187">totalLicenseCount</span></span>|<span data-ttu-id="fdda1-188">Int32</span><span class="sxs-lookup"><span data-stu-id="fdda1-188">Int32</span></span>|<span data-ttu-id="fdda1-189">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="fdda1-189">Total license count.</span></span>|
|<span data-ttu-id="fdda1-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="fdda1-190">usedLicenseCount</span></span>|<span data-ttu-id="fdda1-191">Int32</span><span class="sxs-lookup"><span data-stu-id="fdda1-191">Int32</span></span>|<span data-ttu-id="fdda1-192">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="fdda1-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="fdda1-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdda1-193">Response</span></span>
<span data-ttu-id="fdda1-194">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune_books_iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fdda1-194">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdda1-195">Пример</span><span class="sxs-lookup"><span data-stu-id="fdda1-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdda1-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdda1-196">Request</span></span>
<span data-ttu-id="fdda1-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdda1-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 853

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="fdda1-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdda1-198">Response</span></span>
<span data-ttu-id="fdda1-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdda1-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 961

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```








