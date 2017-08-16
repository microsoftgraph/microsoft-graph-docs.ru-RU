# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="68f6e-101">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="68f6e-101">Upload large files with an upload session</span></span>

<span data-ttu-id="68f6e-p101">Создайте сеанс отправки, чтобы приложение могло отправлять файлы, размер которых не превышает максимальный. С помощью сеанса отправки приложение может отправлять диапазоны файла в последовательных запросах API, что позволяет возобновить передачу, если во время отправки соединение будет разорвано.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequental API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="68f6e-104">Процесс отправки файла с помощью сеанса отправки состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="68f6e-104">To upload a file using an upload session, there are two steps:</span></span>

1. <span data-ttu-id="68f6e-105">[Создание сеанса отправки](#create-an-upload-session).</span><span class="sxs-lookup"><span data-stu-id="68f6e-105">[Create an upload session](#create-an-upload-session)</span></span>
2. <span data-ttu-id="68f6e-106">[Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="68f6e-106">[Upload bytes to the upload session](#upload-bytes-to-the-upload-session)</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68f6e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68f6e-107">Prerequisites</span></span>
<span data-ttu-id="68f6e-108">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="68f6e-108">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="68f6e-109">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="68f6e-109">Files.ReadWrite</span></span>
* <span data-ttu-id="68f6e-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68f6e-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="68f6e-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68f6e-111">Sites.ReadWrite.All</span></span>

> <span data-ttu-id="68f6e-p102">**Примечание.** Разрешение приложения Files.ReadWrite.All пока не поддерживается в этом API. Полная поддержка ожидается в скором времени.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p102">**Note**: The Files.ReadWrite.All application permission is not yet supported on this API. Full support is planned soon.</span></span> 

## <a name="create-an-upload-session"></a><span data-ttu-id="68f6e-114">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="68f6e-114">Create an upload session</span></span>

<span data-ttu-id="68f6e-p103">Чтобы начать отправку большого файла, приложение должно сначала запросить новый сеанс отправки. При этом создается временное место хранения, где сохраняются байты файла, пока он не будет отправлен полностью. После отправки последнего байта файла сеанс отправки завершается, а готовый файл отображается в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p103">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="68f6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68f6e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="68f6e-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68f6e-119">Request body</span></span>
<span data-ttu-id="68f6e-p104">Тело запроса не требуется. Но вы можете указать тело запроса, чтобы предоставить дополнительные данные об отправляемом файле.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p104">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="68f6e-122">Например, вы можете задать необходимые действия для случая, когда имя файла уже используется, указав в теле запроса свойство поведения при конфликтах.</span><span class="sxs-lookup"><span data-stu-id="68f6e-122">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="68f6e-123">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68f6e-123">Optional request headers</span></span>

| <span data-ttu-id="68f6e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="68f6e-124">Name</span></span>       | <span data-ttu-id="68f6e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="68f6e-125">Value</span></span> | <span data-ttu-id="68f6e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="68f6e-126">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68f6e-127">*if-match*</span><span class="sxs-lookup"><span data-stu-id="68f6e-127">*if-match*</span></span> | <span data-ttu-id="68f6e-128">etag</span><span class="sxs-lookup"><span data-stu-id="68f6e-128">etag</span></span>  | <span data-ttu-id="68f6e-129">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадает с текущим значением eTag элемента, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="68f6e-129">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |


### <a name="response"></a><span data-ttu-id="68f6e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f6e-130">Response</span></span>
<span data-ttu-id="68f6e-131">В отклике на этот запрос будут представлены подробные сведения о новом экземпляре [uploadSession](../resources/uploadsession.md) (в том числе URL-адрес для отправки фрагментов файла).</span><span class="sxs-lookup"><span data-stu-id="68f6e-131">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

### <a name="example"></a><span data-ttu-id="68f6e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="68f6e-132">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a><span data-ttu-id="68f6e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f6e-133">Response</span></span> 

<span data-ttu-id="68f6e-134">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68f6e-134">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="68f6e-135">Отправка байтов в сеанс отправки</span><span class="sxs-lookup"><span data-stu-id="68f6e-135">Upload bytes to the upload session</span></span>

<span data-ttu-id="68f6e-p105">Чтобы отправить файл или его часть, приложение выполняет запрос PUT на адрес **uploadUrl**, указанный в отклике для **createUploadSession**. Вы можете отправить файл целиком или разделить его на фрагменты. При этом каждый запрос должен содержать фрагмент размером не более 60 МБ. Фрагменты файла необходимо отправлять в правильном порядке. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p105">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response. You can upload the entire file, or split the file into fragments, as long as the maximum bytes in any given request is less than 60 MiB. The fragments of the file must be uploaded sequentally in order. Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="68f6e-p106">**Примечание.** Если приложение делит файл на несколько фрагментов, размер каждого фрагмента **ДОЛЖЕН** быть кратным 320 КБ. Если размер фрагментов не делится на 320 без остатка, при отправке некоторых файлов возникнут ошибки.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p106">**Note:** If your app splits a file into multiple fragments, the size of each fragment **MUST** be a multiple of 320 KiB. Using a fragment size that does not divide evenly by 320 will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="68f6e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="68f6e-142">Example</span></span>

<span data-ttu-id="68f6e-p107">В этом примере отправляются первые 26 из 128 байтов файла. Заголовок **Content-Length** задает размер текущего запроса. Заголовок **Content-Range** указывает диапазон (в байтах) для всего файла, представленного в запросе. Прежде чем отправлять первый фрагмент файла, необходимо знать общий размер этого файла.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p107">This example is uploading the first 26 bytes of a 128 byte file. The **Content-Length** header specifies the size of the current request. The **Content-Range** header indicates the range of bytes in the overall file that this request represents. The total length of the file must be known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="68f6e-p108">**Важно!** Приложение должно указывать в заголовках **Content-Range** всех запросов один и тот же общий размер файла. Если объявить для фрагмента другой размер файла, запрос не будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p108">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests. If a fragment declares a different file size, the request will fail.</span></span>

##### <a name="response"></a><span data-ttu-id="68f6e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f6e-149">Response</span></span>

<span data-ttu-id="68f6e-150">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68f6e-150">The following example shows the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="68f6e-p109">С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий фрагмент. Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p109">Your app can use the **nextExpectedRanges** value to determine where to start the next fragment. You may see multiple ranges specified, indicating parts of the file that the server has not yet received. This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="68f6e-p110">Размер фрагментов всегда следует определять в соответствии с приведенными ниже рекомендациями. Не рассчитывайте на то, что свойство **nextExpectedRanges** вернет диапазоны надлежащего размера для отправляемого фрагмента. Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p110">You should always determine the fragment size according to the best practices below. Do not assume that **nextExpectedRanges** will return reanges of proper size for an upload fragment. The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how you should upload the file.</span></span>

<span data-ttu-id="68f6e-157">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="68f6e-157">**Notes:**</span></span>

* <span data-ttu-id="68f6e-158">Свойство `nextExpectedRanges` не всегда указывает все отсутствующие диапазоны.</span><span class="sxs-lookup"><span data-stu-id="68f6e-158">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="68f6e-p111">При успешной записи фрагментов оно возвращает следующий диапазон (например, "523-").</span><span class="sxs-lookup"><span data-stu-id="68f6e-p111">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="68f6e-p112">При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#resuming-an-in-progress-upload), чтобы получить более подробный список недостающих диапазонов.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p112">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="68f6e-p113">В ответ на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthoized`. Заголовок авторизации и токен носителя необходимо отправлять только при публикации `POST` на начальном этапе. Не следует включать их, когда совершается вызов `PUT`.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p113">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthoized` response. The Authoization header and bearer token should only be sent when issueing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>   


## <a name="completing-a-file"></a><span data-ttu-id="68f6e-166">Завершение отправки файла</span><span class="sxs-lookup"><span data-stu-id="68f6e-166">Completing a file</span></span>

<span data-ttu-id="68f6e-p114">После получения последнего фрагмента файла сервер отправляет отклик `HTTP 201 Created` или `HTTP 200 OK`. Тело отклика также включает набор свойств по умолчанию для ресурса **driveItem**, представляющего полностью отправленный файл.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p114">When the last fragment of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`. The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
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
<span data-ttu-id="68f6e-169">**Примечание.** Для наглядности отклик элемента усечен.</span><span class="sxs-lookup"><span data-stu-id="68f6e-169">**Note:** The item response is truncated for documentation clarity.</span></span>

## <a name="cancel-an-upload-session"></a><span data-ttu-id="68f6e-170">Отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="68f6e-170">Cancel an upload session</span></span>

<span data-ttu-id="68f6e-p115">Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. При этом очищается временный файл, содержащий ранее отправленные данные. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).</span><span class="sxs-lookup"><span data-stu-id="68f6e-p115">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="68f6e-174">Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="68f6e-174">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="example"></a><span data-ttu-id="68f6e-175">Пример</span><span class="sxs-lookup"><span data-stu-id="68f6e-175">Example</span></span>

<span data-ttu-id="68f6e-176">Запрос DELETE мгновенно останавливает сеанс отправки и удаляет все ранее отправленные байты.</span><span class="sxs-lookup"><span data-stu-id="68f6e-176">The DELETE request will immedately expire the upload session and remove any previously uploaded bytes.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a><span data-ttu-id="68f6e-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f6e-177">Response</span></span> 

<span data-ttu-id="68f6e-178">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68f6e-178">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="68f6e-179">Возобновление выполняемой отправки</span><span class="sxs-lookup"><span data-stu-id="68f6e-179">Resuming an in-progress upload</span></span>

<span data-ttu-id="68f6e-p116">При отключении или сбое отправки до полного выполнения запроса все байты в этом запросе игнорируются. Это может произойти при разрыве соединения между приложением и службой. В этом случае приложение может возобновить передачу файла с ранее отправленного фрагмента.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p116">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="68f6e-183">Чтобы узнать, какие диапазоны байтов были получены ранее, приложение может запросить состояние сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="68f6e-183">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="68f6e-184">Пример</span><span class="sxs-lookup"><span data-stu-id="68f6e-184">Example</span></span>
<span data-ttu-id="68f6e-185">Получить состояние отправки можно, отправив запрос GET на адрес `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="68f6e-185">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

<span data-ttu-id="68f6e-186">В ответ сервер отправит список отсутствующих байтовых диапазонов, которые требуется отправить, и время окончания срока действия для сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="68f6e-186">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="68f6e-187">Отправка оставшихся данных</span><span class="sxs-lookup"><span data-stu-id="68f6e-187">Upload remaining data</span></span>
<span data-ttu-id="68f6e-188">Теперь, когда приложению известно, с какого момента начинать отправку, возобновите операцию, выполнив действия из раздела [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="68f6e-188">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>


## <a name="best-practices"></a><span data-ttu-id="68f6e-189">Советы и рекомендации</span><span class="sxs-lookup"><span data-stu-id="68f6e-189">Best practices</span></span>

* <span data-ttu-id="68f6e-190">Возобновляйте или повторно запускайте операции отправки, не выполненные из-за разрывов соединения или каких-либо ошибок с кодом 5xx, в том числе:</span><span class="sxs-lookup"><span data-stu-id="68f6e-190">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="68f6e-191">Используйте стратегию экспоненциального откладывания, если при возобновлении или повторной отправке возвращаются ошибки сервера с кодом 5xx.</span><span class="sxs-lookup"><span data-stu-id="68f6e-191">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="68f6e-192">При возникновении других ошибок не следует использовать эту стратегию. Вместо этого ограничьте количество повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="68f6e-192">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="68f6e-193">Для устранения ошибок `404 Not Found` при возобновляемой отправке начинайте всю отправку заново.</span><span class="sxs-lookup"><span data-stu-id="68f6e-193">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span>
* <span data-ttu-id="68f6e-194">Используйте возобновляемую отправку для файлов размером более 10 МБ (10 \* 1024 \* 1024 байтов).</span><span class="sxs-lookup"><span data-stu-id="68f6e-194">Use resumable file transfers for files larger than 10 MiB (10 \* 1024 \* 1024 bytes).</span></span>
* <span data-ttu-id="68f6e-p117">Размер 10 МБ для фрагмента оптимален в случае стабильных высокоскоростных подключений. Если используется более медленное или менее надежное подключение, то вы можете достичь оптимальных результатов, используя уменьшенные фрагменты. Рекомендуем использовать фрагменты размером 5–10 МБ.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p117">A fragment size of 10 MiB for stable high speed connections is optimal. For slower or less reliable connections you may get better results from a smaller fragment size. The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="68f6e-p118">Используйте размер фрагментов, кратный 320 КБ (320 \* 1024 байтов). В противном случае после отправки последнего фрагмента большого файла может произойти сбой.</span><span class="sxs-lookup"><span data-stu-id="68f6e-p118">Use a fragment size that is a multiple of 320 KiB (320 \* 1024 bytes). Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last fragment is uploaded.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
