---
<span data-ttu-id="9fd43-101">Автор: Описание JeremyKelley: "Создайте сеанс загрузки, чтобы позволить приложению загружать файлы до максимального размера файла".</span><span class="sxs-lookup"><span data-stu-id="9fd43-101">author: JeremyKelley description: "Create an upload session to allow your app to upload files up to the maximum file size."</span></span>
<span data-ttu-id="9fd43-102">название: driveItem: createUploadSession localization_priority: Normal ms.prod: "sites-and-lists" doc_type: apiPageType</span><span class="sxs-lookup"><span data-stu-id="9fd43-102">title: driveItem: createUploadSession localization_priority: Normal ms.prod: "sites-and-lists" doc_type: apiPageType</span></span>
---
# <a name="driveitem-createuploadsession"></a><span data-ttu-id="9fd43-103">driveItem: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="9fd43-103">driveItem: createUploadSession</span></span>

<span data-ttu-id="9fd43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fd43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd43-105">Создайте сеанс отправки, чтобы приложение могло отправлять файлы, размер которых не превышает максимальный.</span><span class="sxs-lookup"><span data-stu-id="9fd43-105">Create an upload session to allow your app to upload files up to the maximum file size.</span></span>

<span data-ttu-id="9fd43-106">Сеанс загрузки позволяет приложению загружать диапазоны файла в последовательном запросе API, что позволяет возобновить передачу, если подключение отброшено во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-106">An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="9fd43-107">Чтобы загрузить файл с помощью сеанса загрузки:</span><span class="sxs-lookup"><span data-stu-id="9fd43-107">To upload a file using an upload session:</span></span>

1. <span data-ttu-id="9fd43-108">[Создание сеанса отправки](#create-an-upload-session).</span><span class="sxs-lookup"><span data-stu-id="9fd43-108">[Create an upload session](#create-an-upload-session)</span></span>
2. <span data-ttu-id="9fd43-109">[Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="9fd43-109">[Upload bytes to the upload session](#upload-bytes-to-the-upload-session)</span></span>

## <a name="permissions"></a><span data-ttu-id="9fd43-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fd43-110">Permissions</span></span>

<span data-ttu-id="9fd43-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fd43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fd43-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fd43-113">Permission type</span></span>      | <span data-ttu-id="9fd43-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fd43-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fd43-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fd43-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9fd43-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd43-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fd43-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fd43-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fd43-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd43-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fd43-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fd43-119">Application</span></span> | <span data-ttu-id="9fd43-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd43-120">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="9fd43-121">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="9fd43-121">Create an upload session</span></span>

<span data-ttu-id="9fd43-122">Чтобы начать отправку большого файла, приложение должно сначала запросить новый сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-122">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="9fd43-123">При этом создается временное место хранения, где сохраняются байты файла, пока он не будет отправлен полностью.</span><span class="sxs-lookup"><span data-stu-id="9fd43-123">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="9fd43-124">После отправки последнего байта файла сеанс отправки завершается, а готовый файл отображается в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="9fd43-124">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="9fd43-125">Кроме того, вы можете отложить окончательное создание файла в пункте назначения до тех пор, пока вы явным образом не создадите запрос на завершение отправки, указав свойство `deferCommit` в аргументах запроса.</span><span class="sxs-lookup"><span data-stu-id="9fd43-125">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="9fd43-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fd43-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="9fd43-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fd43-127">Request body</span></span>

<span data-ttu-id="9fd43-128">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="9fd43-128">No request body is required.</span></span>
<span data-ttu-id="9fd43-129">Однако вы можете указать свойства в теле запроса, предоставив дополнительные сведения об отправляемом файле, а также выполнив настройку семантики операции передачи.</span><span class="sxs-lookup"><span data-stu-id="9fd43-129">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="9fd43-130">Например, свойство `item` позволяет задать указанные ниже параметры.</span><span class="sxs-lookup"><span data-stu-id="9fd43-130">For example, the `item` property allows setting the following parameters:</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "fail (default) | replace | rename",
  "description": "description",
  "driveItemSource": { "@odata.type": "microsoft.graph.driveItemSource" },
  "fileSize": 1234,
  "name": "filename.txt",
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

<span data-ttu-id="9fd43-131">В приведенном ниже примере выполняется управление поведением, если имя файла уже занято, и дается указание на то, что окончательный файл не следует создавать, пока не будет создан явный запрос на выполнение:</span><span class="sxs-lookup"><span data-stu-id="9fd43-131">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="9fd43-132">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fd43-132">Optional request headers</span></span>

| <span data-ttu-id="9fd43-133">Имя</span><span class="sxs-lookup"><span data-stu-id="9fd43-133">Name</span></span>       | <span data-ttu-id="9fd43-134">Значение</span><span class="sxs-lookup"><span data-stu-id="9fd43-134">Value</span></span> | <span data-ttu-id="9fd43-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd43-135">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9fd43-136">*if-match*</span><span class="sxs-lookup"><span data-stu-id="9fd43-136">*if-match*</span></span> | <span data-ttu-id="9fd43-137">etag</span><span class="sxs-lookup"><span data-stu-id="9fd43-137">etag</span></span>  | <span data-ttu-id="9fd43-138">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадает с текущим значением eTag элемента, то возвращается ошибка `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="9fd43-138">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="9fd43-139">Параметры</span><span class="sxs-lookup"><span data-stu-id="9fd43-139">Parameters</span></span>

| <span data-ttu-id="9fd43-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="9fd43-140">Parameter</span></span>            | <span data-ttu-id="9fd43-141">Тип</span><span class="sxs-lookup"><span data-stu-id="9fd43-141">Type</span></span>                          | <span data-ttu-id="9fd43-142">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd43-142">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="9fd43-143">item</span><span class="sxs-lookup"><span data-stu-id="9fd43-143">item</span></span>                 | [<span data-ttu-id="9fd43-144">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="9fd43-144">driveItemUploadableProperties</span></span>](../resources/driveItemUploadableProperties.md) | <span data-ttu-id="9fd43-145">Сведения об отправляемом файле</span><span class="sxs-lookup"><span data-stu-id="9fd43-145">Data about the file being uploaded</span></span>
| <span data-ttu-id="9fd43-146">deferCommit</span><span class="sxs-lookup"><span data-stu-id="9fd43-146">deferCommit</span></span>          | <span data-ttu-id="9fd43-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fd43-147">Boolean</span></span>                       | <span data-ttu-id="9fd43-148">Если задано значение "true", то для окончательного создания файла в пункте назначения потребуется явный запрос.</span><span class="sxs-lookup"><span data-stu-id="9fd43-148">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="9fd43-149">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9fd43-149">Only on OneDrive for Business.</span></span>

### <a name="request"></a><span data-ttu-id="9fd43-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fd43-150">Request</span></span>

<span data-ttu-id="9fd43-151">В отклике на этот запрос будут представлены подробные сведения о новом экземпляре [uploadSession](../resources/uploadsession.md) (в том числе URL-адрес для отправки фрагментов файла).</span><span class="sxs-lookup"><span data-stu-id="9fd43-151">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="9fd43-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fd43-152">Response</span></span>

<span data-ttu-id="9fd43-153">В случае успешного выполнения запроса ответ будет содержать сведения о том, куда отправлять остальные запросы (в виде ресурса [UploadSession](../resources/uploadsession.md)).</span><span class="sxs-lookup"><span data-stu-id="9fd43-153">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="9fd43-154">Этот ресурс предоставляет сведения о том, куда следует отправлять диапазон байтов файла и когда истекает срок действия сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-154">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<span data-ttu-id="9fd43-155">Если указан параметр `fileSize` и он превышает доступную квоту, то возвращается отклик `507 Insufficent Storage`, а сеанс отправки не будет создан.</span><span class="sxs-lookup"><span data-stu-id="9fd43-155">If the `fileSize` parameter is specified and exceeds the available quota, a `507 Insufficent Storage` response will be returned and the upload session will not be created.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="9fd43-156">Отправка байтов в сеанс отправки</span><span class="sxs-lookup"><span data-stu-id="9fd43-156">Upload bytes to the upload session</span></span>

<span data-ttu-id="9fd43-157">Чтобы отправить файл или его часть, приложение отправляет запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="9fd43-157">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="9fd43-158">Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером не более 60 МБ.</span><span class="sxs-lookup"><span data-stu-id="9fd43-158">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="9fd43-159">Фрагменты файла необходимо отправлять в правильном порядке.</span><span class="sxs-lookup"><span data-stu-id="9fd43-159">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="9fd43-160">В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="9fd43-160">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="9fd43-161">**Примечание.** Если приложение делит файл на несколько диапазонов байтов, размер каждого из них **ДОЛЖЕН** быть кратным 320 КиБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="9fd43-161">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="9fd43-162">Если размер фрагментов не делится на 320 КБ без остатка, при отправке некоторых файлов возникнут ошибки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-162">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="9fd43-163">Пример</span><span class="sxs-lookup"><span data-stu-id="9fd43-163">Example</span></span>

<span data-ttu-id="9fd43-164">В этом примере приложение отправляет первые 26 из 128 байтов файла.</span><span class="sxs-lookup"><span data-stu-id="9fd43-164">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="9fd43-165">Заголовок **Content-Length** задает размер текущего запроса.</span><span class="sxs-lookup"><span data-stu-id="9fd43-165">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="9fd43-166">Заголовок **Content-Range** указывает диапазон байтов для всего файла, представленного в запросе.</span><span class="sxs-lookup"><span data-stu-id="9fd43-166">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="9fd43-167">Прежде чем отправлять первый фрагмент файла, необходимо знать общий размер этого файла.</span><span class="sxs-lookup"><span data-stu-id="9fd43-167">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="9fd43-168">**Важно!** Приложение должно указывать в заголовках **Content-Range** всех запросов один и тот же общий размер файла.</span><span class="sxs-lookup"><span data-stu-id="9fd43-168">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="9fd43-169">Если объявить для диапазона байтов другой размер файла, запрос не будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="9fd43-169">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="9fd43-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fd43-170">Response</span></span>

<span data-ttu-id="9fd43-171">После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.</span><span class="sxs-lookup"><span data-stu-id="9fd43-171">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="9fd43-172">С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="9fd43-172">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="9fd43-173">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="9fd43-173">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="9fd43-174">Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="9fd43-174">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="9fd43-175">Размер диапазонов байтов всегда следует определять в соответствии с приведенными ниже рекомендациями.</span><span class="sxs-lookup"><span data-stu-id="9fd43-175">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="9fd43-176">Не рассчитывайте, что свойство **nextExpectedRanges** вернет диапазоны надлежащего размера для отправляемого диапазона байтов.</span><span class="sxs-lookup"><span data-stu-id="9fd43-176">Do not assume that **nextExpectedRanges** will return ranges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="9fd43-177">Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.</span><span class="sxs-lookup"><span data-stu-id="9fd43-177">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="9fd43-178">Примечания</span><span class="sxs-lookup"><span data-stu-id="9fd43-178">Remarks</span></span>

* <span data-ttu-id="9fd43-179">Свойство `nextExpectedRanges` не всегда указывает все отсутствующие диапазоны.</span><span class="sxs-lookup"><span data-stu-id="9fd43-179">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="9fd43-p112">При успешной записи фрагментов оно возвращает следующий диапазон (например, "523-").</span><span class="sxs-lookup"><span data-stu-id="9fd43-p112">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="9fd43-p113">При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#resuming-an-in-progress-upload), чтобы получить более подробный список недостающих диапазонов.</span><span class="sxs-lookup"><span data-stu-id="9fd43-p113">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="9fd43-p114">Как отклик на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`. Заголовок авторизации и токен носителя необходимо отправлять только при выполнении `POST` на начальном этапе. Не следует включать их, когда совершается вызов `PUT`.</span><span class="sxs-lookup"><span data-stu-id="9fd43-p114">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="9fd43-187">Завершение отправки файла</span><span class="sxs-lookup"><span data-stu-id="9fd43-187">Completing a file</span></span>

<span data-ttu-id="9fd43-188">Если параметр `deferCommit` имеет значение "false" или он не задан, то отправка автоматически завершается, когда последний диапазон байтов файла методом PUT достигает URL-адреса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-188">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>

<span data-ttu-id="9fd43-189">Если параметр `deferCommit` имеет значение "true", то можно явным образом завершить отправку двумя способами:</span><span class="sxs-lookup"><span data-stu-id="9fd43-189">If `deferCommit` is true, you can explicitly complete the upload in two ways:</span></span>
- <span data-ttu-id="9fd43-190">После того как последний диапазон байтов файла методом PUT достигает URL-адреса отправки, отправьте последний запрос POST на URL-адрес отправки с содержимым нулевой длины (в настоящее время поддерживается только в OneDrive для бизнеса и в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="9fd43-190">After the final byte range of the file is PUT to the upload URL, send a final POST request to the upload URL with zero-length content (currently only supported on OneDrive for Business and SharePoint).</span></span>
- <span data-ttu-id="9fd43-191">После того как последний диапазон байтов файла методом PUT достигает URL-адреса отправки, отправьте последний запрос PUT таким же образом, которым вы бы [обрабатывали ошибки отправки](#handle-upload-errors) (в настоящее время поддерживается только в OneDrive персональный).</span><span class="sxs-lookup"><span data-stu-id="9fd43-191">After the final byte range of the file is PUT to the upload URL, send a final PUT request in the same way that you would [handle upload errors](#handle-upload-errors) (currently only supported on OneDrive Personal).</span></span>


<span data-ttu-id="9fd43-192">После завершения отправки сервер ответит на последний запрос со значением `HTTP 201 Created` или `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="9fd43-192">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="9fd43-193">Текст ответа также включает набор свойств по умолчанию для ресурса **driveItem**, представляющего полностью отправленный файл.</span><span class="sxs-lookup"><span data-stu-id="9fd43-193">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```


<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```http
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="handling-upload-conflicts"></a><span data-ttu-id="9fd43-194">Обработка конфликтов при отправке</span><span class="sxs-lookup"><span data-stu-id="9fd43-194">Handling upload conflicts</span></span>

<span data-ttu-id="9fd43-195">В случае возникновения конфликта после отправки файла (например, если в ходе сеанса отправки был создан элемент с таким же именем) при отправке последнего диапазона байтов возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="9fd43-195">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="9fd43-196">Отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="9fd43-196">Cancel the upload session</span></span>

<span data-ttu-id="9fd43-p116">Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. При этом очищается временный файл, содержащий ранее отправленные данные. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).</span><span class="sxs-lookup"><span data-stu-id="9fd43-p116">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="9fd43-200">Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9fd43-200">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="9fd43-201">Временные файлы могут быть удалены не сразу по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="9fd43-201">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="9fd43-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fd43-202">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="9fd43-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fd43-203">Response</span></span>

<span data-ttu-id="9fd43-204">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fd43-204">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="9fd43-205">Возобновление выполняемой отправки</span><span class="sxs-lookup"><span data-stu-id="9fd43-205">Resuming an in-progress upload</span></span>

<span data-ttu-id="9fd43-p118">При отключении или сбое отправки до полного выполнения запроса все байты в этом запросе игнорируются. Это может произойти при разрыве соединения между приложением и службой. В этом случае приложение может возобновить передачу файла с ранее отправленного фрагмента.</span><span class="sxs-lookup"><span data-stu-id="9fd43-p118">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="9fd43-209">Чтобы узнать, какие диапазоны байтов были получены ранее, приложение может запросить состояние сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-209">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="9fd43-210">Пример</span><span class="sxs-lookup"><span data-stu-id="9fd43-210">Example</span></span>

<span data-ttu-id="9fd43-211">Получить состояние отправки можно, отправив запрос GET на адрес `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="9fd43-211">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="9fd43-212">В ответ сервер отправит список отсутствующих байтовых диапазонов, которые требуется отправить, и время окончания срока действия для сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-212">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="9fd43-213">Отправка оставшихся данных</span><span class="sxs-lookup"><span data-stu-id="9fd43-213">Upload remaining data</span></span>

<span data-ttu-id="9fd43-214">Теперь, когда приложению известно, с какого момента начинать отправку, возобновите операцию, выполнив действия из раздела [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="9fd43-214">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="9fd43-215">Обработка ошибок отправки</span><span class="sxs-lookup"><span data-stu-id="9fd43-215">Handle upload errors</span></span>

<span data-ttu-id="9fd43-216">После отправки последнего диапазона байтов файла может возникнуть ошибка.</span><span class="sxs-lookup"><span data-stu-id="9fd43-216">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="9fd43-217">Она может быть вызвана конфликтом имен или превышением ограничения квоты.</span><span class="sxs-lookup"><span data-stu-id="9fd43-217">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="9fd43-218">Сеанс отправки будет сохранен до истечения срока его действия. Это позволяет приложению возобновить отправку, явно зафиксировав сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-218">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="9fd43-219">Для этого приложение должно отправить запрос PUT с новым ресурсом **driveItem**, который будет использоваться при фиксации сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-219">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="9fd43-220">Этот новый запрос должен устранить причину первоначальной ошибки отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-220">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="9fd43-221">Чтобы указать, что приложение применяет существующий сеанс отправки, запрос PUT должен включать свойство `@microsoft.graph.sourceUrl` со значением URL-адреса сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="9fd43-221">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_file}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="9fd43-222">**Примечание.** В этом вызове можно использовать заголовки `@microsoft.graph.conflictBehavior` и `if-match` надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9fd43-222">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="response"></a><span data-ttu-id="9fd43-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fd43-223">Response</span></span>

<span data-ttu-id="9fd43-224">Если файл можно зафиксировать с помощью новых метаданных, возвращается ответ `HTTP 201 Created` или `HTTP 200 OK` с метаданными ресурса Item для отправленного файла.</span><span class="sxs-lookup"><span data-stu-id="9fd43-224">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="best-practices"></a><span data-ttu-id="9fd43-225">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="9fd43-225">Best practices</span></span>

* <span data-ttu-id="9fd43-226">Возобновляйте или повторно запускайте операции отправки, не выполненные из-за разрывов соединения или каких-либо ошибок с кодом 5xx, в том числе:</span><span class="sxs-lookup"><span data-stu-id="9fd43-226">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="9fd43-227">Используйте стратегию экспоненциального откладывания, если при возобновлении или повторной отправке возвращаются ошибки сервера с кодом 5xx.</span><span class="sxs-lookup"><span data-stu-id="9fd43-227">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="9fd43-228">При возникновении других ошибок не следует использовать эту стратегию. Вместо этого ограничьте количество повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="9fd43-228">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="9fd43-229">Для устранения ошибок `404 Not Found` при возобновляемой отправке начинайте всю отправку заново.</span><span class="sxs-lookup"><span data-stu-id="9fd43-229">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="9fd43-230">Это означает, что сеанс отправки больше не существует.</span><span class="sxs-lookup"><span data-stu-id="9fd43-230">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="9fd43-231">Используйте возобновляемую отправку для файлов размером более 10 МБ (10 485 760 байтов).</span><span class="sxs-lookup"><span data-stu-id="9fd43-231">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="9fd43-232">Размер 10 МБ для диапазона байтов оптимален при использовании стабильных высокоскоростных подключений.</span><span class="sxs-lookup"><span data-stu-id="9fd43-232">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="9fd43-233">Если используется более медленное или менее надежное подключение, то вы можете достичь оптимальных результатов, используя фрагменты меньших размеров.</span><span class="sxs-lookup"><span data-stu-id="9fd43-233">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="9fd43-234">Рекомендуем использовать фрагменты размером 5–10 МиБ.</span><span class="sxs-lookup"><span data-stu-id="9fd43-234">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="9fd43-235">Используйте размер фрагментов, кратный 320 КиБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="9fd43-235">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="9fd43-236">В противном случае после отправки последнего диапазона байтов большого файла может произойти сбой.</span><span class="sxs-lookup"><span data-stu-id="9fd43-236">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="9fd43-237">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="9fd43-237">Error responses</span></span>

<span data-ttu-id="9fd43-238">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="9fd43-238">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[driveItemSource]: ../resources/driveItemSource.md
[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[mediaSource]: ../resources/mediaSource.md

<!--
{
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation",
  "suppressions": []
}
-->


