---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Возобновляемая отправка файлов"
ms.openlocfilehash: 39aee7121483e423c4adbd910c80e1ca059c685a
ms.sourcegitcommit: e9b5d370a1d9a03d908dc430994d6a196b1345b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2017
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="81f14-102">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-102">Upload large files with an upload session</span></span>

<span data-ttu-id="81f14-p101">Создайте сеанс отправки, чтобы приложение могло отправлять файлы, размер которых не превышает максимальный. С помощью сеанса отправки приложение может отправлять диапазоны файла при последовательных запросах API, что позволяет возобновить передачу, если во время отправки соединение будет разорвано.</span><span class="sxs-lookup"><span data-stu-id="81f14-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="81f14-105">Процесс отправки файла с помощью сеанса отправки состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="81f14-105">To upload a file using an upload session, there are two steps:</span></span>

1. <span data-ttu-id="81f14-106">[Создание сеанса отправки](#create-an-upload-session).</span><span class="sxs-lookup"><span data-stu-id="81f14-106">[Create an upload session](#create-an-upload-session)</span></span>
2. <span data-ttu-id="81f14-107">[Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="81f14-107">[Upload bytes to the upload session](#upload-bytes-to-the-upload-session)</span></span>

## <a name="permissions"></a><span data-ttu-id="81f14-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81f14-108">Permissions</span></span>

<span data-ttu-id="81f14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81f14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81f14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81f14-111">Permission type</span></span>      | <span data-ttu-id="81f14-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81f14-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81f14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81f14-113">Delegated (work or school account)</span></span> | <span data-ttu-id="81f14-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f14-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="81f14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81f14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81f14-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f14-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="81f14-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81f14-117">Application</span></span> | <span data-ttu-id="81f14-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f14-118">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="81f14-119">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-119">Create an upload session</span></span>

<span data-ttu-id="81f14-p103">Чтобы начать отправку большого файла, приложение должно сначала запросить новый сеанс отправки. При этом создается временное место хранения, где сохраняются байты файла, пока он не будет отправлен полностью. После отправки последнего байта файла сеанс отправки завершается, а готовый файл отображается в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="81f14-p103">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="81f14-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81f14-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="81f14-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81f14-124">Request body</span></span>

<span data-ttu-id="81f14-p104">Тело запроса не требуется. Но вы можете указать тело запроса, чтобы предоставить дополнительные данные об отправляемом файле.</span><span class="sxs-lookup"><span data-stu-id="81f14-p104">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="81f14-127">Например, вы можете задать необходимые действия для случая, когда имя файла уже используется, указав в теле запроса свойство поведения при конфликтах.</span><span class="sxs-lookup"><span data-stu-id="81f14-127">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="81f14-128">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81f14-128">Optional request headers</span></span>

| <span data-ttu-id="81f14-129">Имя</span><span class="sxs-lookup"><span data-stu-id="81f14-129">Name</span></span>       | <span data-ttu-id="81f14-130">Значение</span><span class="sxs-lookup"><span data-stu-id="81f14-130">Value</span></span> | <span data-ttu-id="81f14-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81f14-131">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="81f14-132">*if-match*</span><span class="sxs-lookup"><span data-stu-id="81f14-132">*if-match*</span></span> | <span data-ttu-id="81f14-133">etag</span><span class="sxs-lookup"><span data-stu-id="81f14-133">etag</span></span>  | <span data-ttu-id="81f14-134">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадает с текущим значением eTag элемента, то возвращается ошибка `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="81f14-134">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |

### <a name="request"></a><span data-ttu-id="81f14-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="81f14-135">Request</span></span>

<span data-ttu-id="81f14-136">В отклике на этот запрос будут представлены подробные сведения о новом экземпляре [uploadSession](../resources/uploadsession.md) (в том числе URL-адрес для отправки фрагментов файла).</span><span class="sxs-lookup"><span data-stu-id="81f14-136">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="81f14-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f14-137">Response</span></span>

<span data-ttu-id="81f14-138">В случае успешного выполнения запроса ответ будет содержать сведения о том, куда отправлять остальные запросы (в виде ресурса [UploadSession](../resources/uploadSession.md)).</span><span class="sxs-lookup"><span data-stu-id="81f14-138">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadSession.md) resource.</span></span>

<span data-ttu-id="81f14-139">Этот ресурс предоставляет сведения о том, куда следует отправлять диапазон байтов файла и когда истекает срок действия сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-139">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

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

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="81f14-140">Отправка байтов в сеанс отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-140">Upload bytes to the upload session</span></span>

<span data-ttu-id="81f14-141">Чтобы отправить файл или его часть, приложение отправляет запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="81f14-141">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="81f14-142">Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером не более 60 МБ.</span><span class="sxs-lookup"><span data-stu-id="81f14-142">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="81f14-143">Фрагменты файла необходимо отправлять в правильном порядке.</span><span class="sxs-lookup"><span data-stu-id="81f14-143">The fragments of the file must be uploaded sequentally in order.</span></span>
<span data-ttu-id="81f14-144">В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="81f14-144">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="81f14-145">**Примечание.** Если приложение делит файл на несколько диапазонов байтов, размер каждого из них **ДОЛЖЕН** быть кратным 320 КиБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="81f14-145">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="81f14-146">Если размер фрагментов не делится на 320 КБ без остатка, при отправке некоторых файлов возникнут ошибки.</span><span class="sxs-lookup"><span data-stu-id="81f14-146">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="81f14-147">Пример</span><span class="sxs-lookup"><span data-stu-id="81f14-147">Example</span></span>

<span data-ttu-id="81f14-148">В этом примере приложение отправляет первые 26 из 128 байтов файла.</span><span class="sxs-lookup"><span data-stu-id="81f14-148">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="81f14-149">Заголовок **Content-Length** задает размер текущего запроса.</span><span class="sxs-lookup"><span data-stu-id="81f14-149">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="81f14-150">Заголовок **Content-Range** указывает диапазон байтов для всего файла, представленного в запросе.</span><span class="sxs-lookup"><span data-stu-id="81f14-150">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="81f14-151">Прежде чем отправлять первый фрагмент файла, необходимо знать общий размер этого файла.</span><span class="sxs-lookup"><span data-stu-id="81f14-151">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="81f14-152">**Важно!** Приложение должно указывать в заголовках **Content-Range** всех запросов один и тот же общий размер файла.</span><span class="sxs-lookup"><span data-stu-id="81f14-152">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="81f14-153">Если объявить для диапазона байтов другой размер файла, запрос не будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="81f14-153">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="81f14-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f14-154">Response</span></span>

<span data-ttu-id="81f14-155">После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.</span><span class="sxs-lookup"><span data-stu-id="81f14-155">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="81f14-156">С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="81f14-156">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="81f14-157">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="81f14-157">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="81f14-158">Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="81f14-158">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="81f14-159">Размер диапазонов байтов всегда следует определять в соответствии с приведенными ниже рекомендациями.</span><span class="sxs-lookup"><span data-stu-id="81f14-159">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="81f14-160">Не рассчитывайте на то, что свойство **nextExpectedRanges** вернет диапазоны надлежащего размера для отправляемого диапазона байтов.</span><span class="sxs-lookup"><span data-stu-id="81f14-160">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="81f14-161">Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.</span><span class="sxs-lookup"><span data-stu-id="81f14-161">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="81f14-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="81f14-162">Remarks</span></span>

* <span data-ttu-id="81f14-163">Свойство `nextExpectedRanges` не всегда указывает все отсутствующие диапазоны.</span><span class="sxs-lookup"><span data-stu-id="81f14-163">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="81f14-p111">При успешной записи фрагментов оно возвращает следующий диапазон (например, "523-").</span><span class="sxs-lookup"><span data-stu-id="81f14-p111">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="81f14-p112">При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#resuming-an-in-progress-upload), чтобы получить более подробный список недостающих диапазонов.</span><span class="sxs-lookup"><span data-stu-id="81f14-p112">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="81f14-p113">Как отклик на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`. Заголовок авторизации и токен носителя необходимо отправлять только при выполнении `POST` на начальном этапе. Не следует включать их, когда совершается вызов `PUT`.</span><span class="sxs-lookup"><span data-stu-id="81f14-p113">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="81f14-171">Завершение отправки файла</span><span class="sxs-lookup"><span data-stu-id="81f14-171">Completing a file</span></span>

<span data-ttu-id="81f14-172">После получения последнего диапазона байтов файла сервер отправляет ответ `HTTP 201 Created` или `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="81f14-172">When the last byte range of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="81f14-173">Текст ответа также включает набор свойств по умолчанию для ресурса **driveItem**, представляющего полностью отправленный файл.</span><span class="sxs-lookup"><span data-stu-id="81f14-173">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
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

## <a name="handling-upload-conflicts"></a><span data-ttu-id="81f14-174">Обработка конфликтов при отправке</span><span class="sxs-lookup"><span data-stu-id="81f14-174">Handling upload conflicts</span></span>

<span data-ttu-id="81f14-175">В случае возникновения конфликта после отправки файла (например, если в ходе сеанса отправки был создан элемент с таким же именем) при отправке последнего диапазона байтов возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="81f14-175">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

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

## <a name="cancel-the-upload-session"></a><span data-ttu-id="81f14-176">Отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-176">Cancel the upload session</span></span>

<span data-ttu-id="81f14-p115">Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. При этом очищается временный файл, содержащий ранее отправленные данные. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).</span><span class="sxs-lookup"><span data-stu-id="81f14-p115">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="81f14-180">Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="81f14-180">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="81f14-181">Временные файлы могут быть удалены не сразу по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="81f14-181">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="81f14-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="81f14-182">Request</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="81f14-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="81f14-183">Response</span></span>

<span data-ttu-id="81f14-184">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81f14-184">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="81f14-185">Возобновление выполняемой отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-185">Resuming an in-progress upload</span></span>

<span data-ttu-id="81f14-p117">При отключении или сбое отправки до полного выполнения запроса все байты в этом запросе игнорируются. Это может произойти при разрыве соединения между приложением и службой. В этом случае приложение может возобновить передачу файла с ранее отправленного фрагмента.</span><span class="sxs-lookup"><span data-stu-id="81f14-p117">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="81f14-189">Чтобы узнать, какие диапазоны байтов были получены ранее, приложение может запросить состояние сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-189">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="81f14-190">Пример</span><span class="sxs-lookup"><span data-stu-id="81f14-190">Example</span></span>

<span data-ttu-id="81f14-191">Получить состояние отправки можно, отправив запрос GET на адрес `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="81f14-191">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="81f14-192">В ответ сервер отправит список отсутствующих байтовых диапазонов, которые требуется отправить, и время окончания срока действия для сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-192">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="81f14-193">Отправка оставшихся данных</span><span class="sxs-lookup"><span data-stu-id="81f14-193">Upload remaining data</span></span>

<span data-ttu-id="81f14-194">Теперь, когда приложению известно, с какого момента начинать отправку, возобновите операцию, выполнив действия из раздела [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="81f14-194">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="81f14-195">Обработка ошибок отправки</span><span class="sxs-lookup"><span data-stu-id="81f14-195">Handle upload errors</span></span>

<span data-ttu-id="81f14-196">После отправки последнего диапазона байтов файла может возникнуть ошибка.</span><span class="sxs-lookup"><span data-stu-id="81f14-196">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="81f14-197">Она может быть вызвана конфликтом имен или превышением ограничения квоты.</span><span class="sxs-lookup"><span data-stu-id="81f14-197">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="81f14-198">Сеанс отправки будет сохранен до истечения срока его действия. Это позволяет приложению возобновить отправку, явно зафиксировав сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-198">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="81f14-199">Для этого приложение должно отправить запрос PUT с новым ресурсом **driveItem**, который будет использоваться при фиксации сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-199">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="81f14-200">Этот новый запрос должен устранить причину первоначальной ошибки отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-200">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="81f14-201">Чтобы указать, что приложение применяет существующий сеанс отправки, запрос PUT должен включать свойство `@microsoft.graph.sourceUrl` со значением URL-адреса сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="81f14-201">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile_2.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="81f14-202">**Примечание.** В этом вызове можно использовать заголовки `@microsoft.graph.conflictBehavior` и `if-match` надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81f14-202">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="http-response"></a><span data-ttu-id="81f14-203">HTTP-ответ</span><span class="sxs-lookup"><span data-stu-id="81f14-203">HTTP response</span></span>

<span data-ttu-id="81f14-204">Если файл можно зафиксировать с помощью новых метаданных, возвращается ответ `HTTP 201 Created` или `HTTP 200 OK` с метаданными ресурса Item для отправленного файла.</span><span class="sxs-lookup"><span data-stu-id="81f14-204">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

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

## <a name="best-practices"></a><span data-ttu-id="81f14-205">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="81f14-205">Best practices</span></span>

* <span data-ttu-id="81f14-206">Возобновляйте или повторно запускайте операции отправки, не выполненные из-за разрывов соединения или каких-либо ошибок с кодом 5xx, в том числе:</span><span class="sxs-lookup"><span data-stu-id="81f14-206">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="81f14-207">Используйте стратегию экспоненциального откладывания, если при возобновлении или повторной отправке возвращаются ошибки сервера с кодом 5xx.</span><span class="sxs-lookup"><span data-stu-id="81f14-207">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="81f14-208">При возникновении других ошибок не следует использовать эту стратегию. Вместо этого ограничьте количество повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="81f14-208">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="81f14-209">Для устранения ошибок `404 Not Found` при возобновляемой отправке начинайте всю отправку заново.</span><span class="sxs-lookup"><span data-stu-id="81f14-209">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="81f14-210">Это означает, что сеанс отправки больше не существует.</span><span class="sxs-lookup"><span data-stu-id="81f14-210">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="81f14-211">Используйте возобновляемую отправку для файлов размером более 10 МБ (10 485 760 байтов).</span><span class="sxs-lookup"><span data-stu-id="81f14-211">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="81f14-212">Размер 10 МБ для диапазона байтов оптимален при использовании стабильных высокоскоростных подключений.</span><span class="sxs-lookup"><span data-stu-id="81f14-212">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="81f14-213">Если используется более медленное или менее надежное подключение, то вы можете достичь оптимальных результатов, используя фрагменты меньших размеров.</span><span class="sxs-lookup"><span data-stu-id="81f14-213">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="81f14-214">Рекомендуем использовать фрагменты размером 5–10 МиБ.</span><span class="sxs-lookup"><span data-stu-id="81f14-214">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="81f14-215">Используйте размер фрагментов, кратный 320 КиБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="81f14-215">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="81f14-216">В противном случае после отправки последнего диапазона байтов большого файла может произойти сбой.</span><span class="sxs-lookup"><span data-stu-id="81f14-216">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="81f14-217">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="81f14-217">Error responses</span></span>

<span data-ttu-id="81f14-218">Дополнительные сведения о том как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="81f14-218">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
