# <a name="update-iosvppebook"></a><span data-ttu-id="a8ccb-101">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="a8ccb-101">Update iosVppEBook</span></span>

> <span data-ttu-id="a8ccb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8ccb-103">Обновление свойств объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-103">Update the properties of a [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8ccb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8ccb-104">Prerequisites</span></span>
<span data-ttu-id="a8ccb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8ccb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8ccb-107">Permission type</span></span>|<span data-ttu-id="a8ccb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8ccb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8ccb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8ccb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a8ccb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8ccb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8ccb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8ccb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8ccb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-112">Not supported.</span></span>|
|<span data-ttu-id="a8ccb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8ccb-113">Application</span></span>|<span data-ttu-id="a8ccb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8ccb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8ccb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="a8ccb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8ccb-116">Request headers</span></span>
|<span data-ttu-id="a8ccb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8ccb-117">Header</span></span>|<span data-ttu-id="a8ccb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a8ccb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8ccb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8ccb-119">Authorization</span></span>|<span data-ttu-id="a8ccb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a8ccb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8ccb-121">Принять</span><span class="sxs-lookup"><span data-stu-id="a8ccb-121">Accept</span></span>|<span data-ttu-id="a8ccb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a8ccb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8ccb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8ccb-123">Request body</span></span>
<span data-ttu-id="a8ccb-124">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune_books_iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-124">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>

<span data-ttu-id="a8ccb-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-125">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune_books_iosvppebook.md).</span></span>

|<span data-ttu-id="a8ccb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8ccb-126">Property</span></span>|<span data-ttu-id="a8ccb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ccb-127">Type</span></span>|<span data-ttu-id="a8ccb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ccb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8ccb-129">ИД</span><span class="sxs-lookup"><span data-stu-id="a8ccb-129">id</span></span>|<span data-ttu-id="a8ccb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-130">String</span></span>|<span data-ttu-id="a8ccb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-131">Key of the entity.</span></span> <span data-ttu-id="a8ccb-132">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a8ccb-133">displayName</span></span>|<span data-ttu-id="a8ccb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-134">String</span></span>|<span data-ttu-id="a8ccb-135">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-135">Name of the eBook.</span></span> <span data-ttu-id="a8ccb-136">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-137">описание</span><span class="sxs-lookup"><span data-stu-id="a8ccb-137">description</span></span>|<span data-ttu-id="a8ccb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-138">String</span></span>|<span data-ttu-id="a8ccb-139">Описание.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-139">Description.</span></span> <span data-ttu-id="a8ccb-140">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-141">publisher</span><span class="sxs-lookup"><span data-stu-id="a8ccb-141">publisher</span></span>|<span data-ttu-id="a8ccb-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-142">String</span></span>|<span data-ttu-id="a8ccb-143">Издатель.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-143">Publisher.</span></span> <span data-ttu-id="a8ccb-144">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ccb-145">publishedDateTime</span></span>|<span data-ttu-id="a8ccb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ccb-146">DateTimeOffset</span></span>|<span data-ttu-id="a8ccb-147">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="a8ccb-148">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="a8ccb-149">largeCover</span></span>|[<span data-ttu-id="a8ccb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a8ccb-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="a8ccb-151">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-151">Book cover.</span></span> <span data-ttu-id="a8ccb-152">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ccb-153">createdDateTime</span></span>|<span data-ttu-id="a8ccb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ccb-154">DateTimeOffset</span></span>|<span data-ttu-id="a8ccb-155">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="a8ccb-156">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ccb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a8ccb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ccb-158">DateTimeOffset</span></span>|<span data-ttu-id="a8ccb-159">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="a8ccb-160">Унаследован от объекта [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a8ccb-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a8ccb-161">informationUrl</span></span>|<span data-ttu-id="a8ccb-162">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-162">String</span></span>|<span data-ttu-id="a8ccb-163">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-163">The more information Url.</span></span> <span data-ttu-id="a8ccb-164">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a8ccb-165">privacyInformationUrl</span></span>|<span data-ttu-id="a8ccb-166">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-166">String</span></span>|<span data-ttu-id="a8ccb-167">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-167">The privacy statement Url.</span></span> <span data-ttu-id="a8ccb-168">Наследуется от [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="a8ccb-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="a8ccb-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="a8ccb-169">vppTokenId</span></span>|<span data-ttu-id="a8ccb-170">Guid</span><span class="sxs-lookup"><span data-stu-id="a8ccb-170">Guid</span></span>|<span data-ttu-id="a8ccb-171">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="a8ccb-172">appleId</span><span class="sxs-lookup"><span data-stu-id="a8ccb-172">appleId</span></span>|<span data-ttu-id="a8ccb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-173">String</span></span>|<span data-ttu-id="a8ccb-174">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="a8ccb-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a8ccb-175">vppOrganizationName</span></span>|<span data-ttu-id="a8ccb-176">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-176">String</span></span>|<span data-ttu-id="a8ccb-177">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="a8ccb-178">жанры</span><span class="sxs-lookup"><span data-stu-id="a8ccb-178">genres</span></span>|<span data-ttu-id="a8ccb-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8ccb-179">String collection</span></span>|<span data-ttu-id="a8ccb-180">Жанры.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-180">Genres.</span></span>|
|<span data-ttu-id="a8ccb-181">язык</span><span class="sxs-lookup"><span data-stu-id="a8ccb-181">language</span></span>|<span data-ttu-id="a8ccb-182">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-182">String</span></span>|<span data-ttu-id="a8ccb-183">Язык.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-183">Language.</span></span>|
|<span data-ttu-id="a8ccb-184">продавец</span><span class="sxs-lookup"><span data-stu-id="a8ccb-184">seller</span></span>|<span data-ttu-id="a8ccb-185">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ccb-185">String</span></span>|<span data-ttu-id="a8ccb-186">Продавец.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-186">Seller.</span></span>|
|<span data-ttu-id="a8ccb-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a8ccb-187">totalLicenseCount</span></span>|<span data-ttu-id="a8ccb-188">Int32</span><span class="sxs-lookup"><span data-stu-id="a8ccb-188">Int32</span></span>|<span data-ttu-id="a8ccb-189">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-189">Total license count.</span></span>|
|<span data-ttu-id="a8ccb-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a8ccb-190">usedLicenseCount</span></span>|<span data-ttu-id="a8ccb-191">Int32</span><span class="sxs-lookup"><span data-stu-id="a8ccb-191">Int32</span></span>|<span data-ttu-id="a8ccb-192">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="a8ccb-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8ccb-193">Response</span></span>
<span data-ttu-id="a8ccb-194">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune_books_iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-194">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8ccb-195">Пример</span><span class="sxs-lookup"><span data-stu-id="a8ccb-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8ccb-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8ccb-196">Request</span></span>
<span data-ttu-id="a8ccb-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 803

{
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
  "vppTokenId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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

### <a name="response"></a><span data-ttu-id="a8ccb-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8ccb-198">Response</span></span>
<span data-ttu-id="a8ccb-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8ccb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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
  "vppTokenId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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



