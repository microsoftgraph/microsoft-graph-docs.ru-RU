---
title: Вложение крупных файлов в сообщения Outlook
description: В зависимости от размера файла можно выбрать один из двух способов вложения файла в сообщение.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 5f6f54adf38c0f2827b587e6646df4cb3549a204
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448573"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a><span data-ttu-id="0c18c-103">Прикрепление крупных файлов к сообщениям Outlook в виде вложений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="0c18c-103">Attach large files to Outlook messages as attachments (preview)</span></span>

<span data-ttu-id="0c18c-104">В зависимости от размера файла можно выбрать один из двух способов вложения файлов в [сообщения](/graph/api/resources/message?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0c18c-104">Depending on the size of the file, you can choose one of two ways to attach a file to a [message](/graph/api/resources/message?view=graph-rest-beta):</span></span>

- <span data-ttu-id="0c18c-105">Если размер файла меньше 3 МБ, можно выполнить одну операцию [POST для свойства навигации вложений сообщения](/graph/api/message-post-attachments?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0c18c-105">If the file size is under 3 MB, you can do a single [POST on the attachments navigation property of the message](/graph/api/message-post-attachments?view=graph-rest-beta).</span></span> <span data-ttu-id="0c18c-106">Успешный отклик `POST` включает ИД файла, прикрепленного к сообщению.</span><span class="sxs-lookup"><span data-stu-id="0c18c-106">The successful `POST` response includes the ID of the file attached to the message.</span></span>
- <span data-ttu-id="0c18c-107">Если размер файла составляет от 3 до 150 МБ, создайте сеанс отправки и итеративно используйте `PUT` для отправки диапазонов байтов, пока не будет отправлен весь файл.</span><span class="sxs-lookup"><span data-stu-id="0c18c-107">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="0c18c-108">Заголовок в итоговом успешном отклике `PUT` включает URL-адрес с ИД вложения.</span><span class="sxs-lookup"><span data-stu-id="0c18c-108">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span> 

<span data-ttu-id="0c18c-109">Чтобы вложить в сообщение несколько файлов, выберите способ для каждого файла на основе их размеров и вложите их по отдельности.</span><span class="sxs-lookup"><span data-stu-id="0c18c-109">To attach multiple files to a message, choose the approach for each file based on its file size and attach them individually.</span></span>

<span data-ttu-id="0c18c-110">В этой статье используется пример для иллюстрации второго подхода.</span><span class="sxs-lookup"><span data-stu-id="0c18c-110">This article uses an example to illustrate the second approach.</span></span> <span data-ttu-id="0c18c-111">В этом примере создается и используется сеанс отправки, чтобы добавить большой файл (размером свыше 3 МБ) к определенному сообщению в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="0c18c-111">The example creates and uses an upload session to add a large file attachment (of size over 3MB) to a specific message.</span></span> <span data-ttu-id="0c18c-112">После успешной отправки всего файла возвращается URL-адрес с ИД вложения, с которыми можно выполнять другие операции, например получать метаданные о вложенном файле.</span><span class="sxs-lookup"><span data-stu-id="0c18c-112">Upon successfully uploading the entire file, it gets a URL that contains an ID for the file attachment, with which it can do other operations such as getting the file attachment metadata.</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="0c18c-113">Обратите внимание на [известную проблему](known-issues.md#attaching-large-files-to-messages) при вложении больших файлов в сообщение в общем или делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0c18c-113">Be aware of a [known issue](known-issues.md#attaching-large-files-to-messages) if you're attaching large files to a message in a shared or delegated mailbox.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="0c18c-114">Шаг 1. Создайте сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="0c18c-114">Step 1: Create an upload session</span></span>

<span data-ttu-id="0c18c-115">[Создайте сеанс отправки](/graph/api/attachment-createuploadsession?view=graph-rest-beta), чтобы вложить файл в сообщение.</span><span class="sxs-lookup"><span data-stu-id="0c18c-115">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-beta) to attach a file to a message.</span></span> <span data-ttu-id="0c18c-116">Укажите файл во входном параметре **AttachmentItem**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-116">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="0c18c-117">После успешной операции возвращается `HTTP 201 Created` и новый экземпляр объекта [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta), содержащий непрозрачный URL-адрес, который можно использовать в последующих операциях `PUT` для отправки частей этого файла.</span><span class="sxs-lookup"><span data-stu-id="0c18c-117">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="0c18c-118">Этот экземпляр **uploadSession** предоставляет временное место хранения, где байты файла сохраняются до отправки всего файла.</span><span class="sxs-lookup"><span data-stu-id="0c18c-118">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="0c18c-119">Обязательно запросите разрешение `Mail.ReadWrite` на создание экземпляра **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-119">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession**.</span></span> <span data-ttu-id="0c18c-120">Непрозрачный URL-адрес, возвращенный свойством **uploadUrl** нового объекта **uploadSession**, проходит предварительную проверку подлинности и содержит соответствующий маркер авторизации для последующих запросов `PUT` в домене `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-120">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="0c18c-121">Этот маркер истекает в срок **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-121">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="0c18c-122">Не следует изменять этот URL-адрес для операций `PUT`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-122">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="0c18c-123">Объект **uploadSession** в отклике также включает свойство **nextExpectedRanges**, указывающее, что начальное место отправки должно быть байтом 0.</span><span class="sxs-lookup"><span data-stu-id="0c18c-123">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-request-create-an-upload-session"></a><span data-ttu-id="0c18c-124">Пример запроса: создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="0c18c-124">Example request: create an upload session</span></span>

# <a name="http"></a>[<span data-ttu-id="0c18c-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c18c-125">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="0c18c-126">C#</span><span class="sxs-lookup"><span data-stu-id="0c18c-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c18c-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c18c-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c18c-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c18c-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a><span data-ttu-id="0c18c-129">Пример отклика: получение объекта uploadSession</span><span class="sxs-lookup"><span data-stu-id="0c18c-129">Example response: get an uploadSession object</span></span>
<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="0c18c-130">Шаг 2. Используйте сеанс отправки, чтобы отправить диапазон байтов файла.</span><span class="sxs-lookup"><span data-stu-id="0c18c-130">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="0c18c-131">Чтобы отправить файл или часть файла, сделайте запрос `PUT` к значению свойства **uploadUrl**, возвращенному в составе **uploadSession** на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="0c18c-131">To upload the file, or a portion of the file, make a `PUT` request to the **uploadUrl** property value returned as part of the **uploadSession** in step 1.</span></span> <span data-ttu-id="0c18c-132">Можно отправить файл целиком или разделить файл на несколько диапазонов байтов.</span><span class="sxs-lookup"><span data-stu-id="0c18c-132">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="0c18c-133">Для более высокой производительности размер каждого диапазона байтов не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="0c18c-133">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="0c18c-134">Укажите заголовки и основной текст запроса, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="0c18c-134">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="0c18c-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c18c-135">Request headers</span></span>

| <span data-ttu-id="0c18c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="0c18c-136">Name</span></span>       | <span data-ttu-id="0c18c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0c18c-137">Type</span></span> | <span data-ttu-id="0c18c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0c18c-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c18c-139">Content-Length</span><span class="sxs-lookup"><span data-stu-id="0c18c-139">Content-Length</span></span> | <span data-ttu-id="0c18c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0c18c-140">Int32</span></span> | <span data-ttu-id="0c18c-141">Количество байтов, отправляемых в этой операции.</span><span class="sxs-lookup"><span data-stu-id="0c18c-141">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="0c18c-142">Для более высокой производительности количество байт в каждой операции `PUT` не должно превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="0c18c-142">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="0c18c-143">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="0c18c-143">Required.</span></span> |
| <span data-ttu-id="0c18c-144">Content-Range</span><span class="sxs-lookup"><span data-stu-id="0c18c-144">Content-Range</span></span> | <span data-ttu-id="0c18c-145">String</span><span class="sxs-lookup"><span data-stu-id="0c18c-145">String</span></span> | <span data-ttu-id="0c18c-146">Диапазон байтов файла, отправляемого в этой операции, начиная с байта 0, выраженный в формате `bytes {start}-{end}/{total}`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-146">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="0c18c-147">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="0c18c-147">Required.</span></span> |
| <span data-ttu-id="0c18c-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c18c-148">Content-Type</span></span> | <span data-ttu-id="0c18c-149">String</span><span class="sxs-lookup"><span data-stu-id="0c18c-149">String</span></span>  | <span data-ttu-id="0c18c-150">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="0c18c-150">The MIME type.</span></span> <span data-ttu-id="0c18c-151">Укажите `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-151">Specify `application/octet-stream`.</span></span> <span data-ttu-id="0c18c-152">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="0c18c-152">Required.</span></span> |

<span data-ttu-id="0c18c-153">Не указывайте заголовок запроса `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-153">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="0c18c-154">Запрос `PUT` использует прошедший предварительную проверку подлинности URL-адрес из свойства **uploadUrl**, что позволяет получить доступ к домену `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-154">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="0c18c-155">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c18c-155">Request body</span></span>

<span data-ttu-id="0c18c-156">Укажите фактические байты вкладываемого файла, находящиеся в диапазоне расположения, указанном в заголовке запроса `Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-156">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="0c18c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c18c-157">Response</span></span>
<span data-ttu-id="0c18c-158">После успешной отправки возвращается `HTTP 200 OK` и объект **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-158">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="0c18c-159">Объект отклика имеет указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="0c18c-159">Note the following in the response object:</span></span>

- <span data-ttu-id="0c18c-160">Свойство **ExpirationDateTime** указывает дату и время окончания срока действия для маркера авторизации, внедренного в значение свойства **uploadUrl**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-160">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="0c18c-161">Это значение даты и времени окончания срока действия остается таким же, какое было возвращено начальным объектом **uploadSession** на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="0c18c-161">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="0c18c-162">Свойство **NextExpectedRanges** указывает расположение следующего байта, с которого необходимо начать отправку, например `"NextExpectedRanges":["2097152"]`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-162">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="0c18c-163">Байты файла необходимо отправлять по порядку.</span><span class="sxs-lookup"><span data-stu-id="0c18c-163">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="0c18c-164">Свойство **uploadUrl** не возвращается явным образом, поскольку все операции `PUT` сеанса отправки используют тот же самый URL-адрес, который был возвращен при создании сеанса (на шаге 1).</span><span class="sxs-lookup"><span data-stu-id="0c18c-164">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-request-first-upload"></a><span data-ttu-id="0c18c-165">Пример запроса: первая отправка</span><span class="sxs-lookup"><span data-stu-id="0c18c-165">Example request: first upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a><span data-ttu-id="0c18c-166">Пример отклика: получение начала следующего диапазона байтов, ожидаемого сервером</span><span class="sxs-lookup"><span data-stu-id="0c18c-166">Example response: get the start of the next byte range that the server expects</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="0c18c-167">Шаг 3. Продолжение отправки диапазонов байтов вплоть до отправки всего файла.</span><span class="sxs-lookup"><span data-stu-id="0c18c-167">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="0c18c-168">После первоначальной отправки на шаге 2 продолжайте отправлять оставшиеся части файла, используя аналогичный запрос `PUT`, как описано на шаге 2, до достижения даты и времени окончания срока действия сеанса.</span><span class="sxs-lookup"><span data-stu-id="0c18c-168">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="0c18c-169">Получайте значение **NextExpectedRanges**, чтобы определить, с какого места должен начинаться следующий диапазон байтов для отправки.</span><span class="sxs-lookup"><span data-stu-id="0c18c-169">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="0c18c-170">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="0c18c-170">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="0c18c-171">Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="0c18c-171">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="0c18c-172">После успешной отправки последнего байта файла операция `PUT` возвращает `HTTP 201 Created` и заголовок `Location`, указывающий URL-адрес вложенного файла в домене `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-172">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="0c18c-173">Можно получить ИД вложения по этому URL-адресу и сохранить его для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="0c18c-173">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="0c18c-174">В зависимости от сценария можно использовать этот ИД для [получения метаданных вложения](/graph/api/attachment-get?view=graph-rest-beta) или для [удаления уложения из сообщения](/graph/api/attachment-delete?view=graph-rest-beta) с помощью конечной точки Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0c18c-174">Depending on your scneario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-beta), or [remove the attachment from the message](/graph/api/attachment-delete?view=graph-rest-beta) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="0c18c-175">В следующем примере показана отправка последнего байтового диапазона файла.</span><span class="sxs-lookup"><span data-stu-id="0c18c-175">The following example shows uploading the last byte range of the file.</span></span>

### <a name="example-request-final-upload"></a><span data-ttu-id="0c18c-176">Пример запроса: окончательная отправка</span><span class="sxs-lookup"><span data-stu-id="0c18c-176">Example request: final upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a><span data-ttu-id="0c18c-177">Пример отклика: получения заголовка отклика Location для сохранения ИД вложения.</span><span class="sxs-lookup"><span data-stu-id="0c18c-177">Example response: get the Location response header to save the attachment ID</span></span>

<span data-ttu-id="0c18c-178">URL-адрес, указанный заголовком отклика `Location`, содержит ИД вложения (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`). Сохраните его для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="0c18c-178">From the URL specified by the `Location` response header, save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a><span data-ttu-id="0c18c-179">Шаг 4 (необязательно). Получение вложенного файла из сообщения.</span><span class="sxs-lookup"><span data-stu-id="0c18c-179">Step 4 (optional): Get the file attachment from the message</span></span>

<span data-ttu-id="0c18c-180">Как всегда, при [получении вложения](/graph/api/attachment-get?view=graph-rest-beta) из сообщения размер вложения не ограничивается технически.</span><span class="sxs-lookup"><span data-stu-id="0c18c-180">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-beta) from a message is not technically limited by attachment size.</span></span>

<span data-ttu-id="0c18c-181">Тем не менее, получение большого вложенного файла в формате кодировки base64 влияет на производительность API.</span><span class="sxs-lookup"><span data-stu-id="0c18c-181">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="0c18c-182">Если ожидается вложение большого размера:</span><span class="sxs-lookup"><span data-stu-id="0c18c-182">If you expect a large attachment:</span></span>

- <span data-ttu-id="0c18c-183">Вместо получения вложенного содержимого в формате base64 можно [получить необработанные данные вложенного файла](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="0c18c-183">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="0c18c-184">Чтобы [получить метаданные вложенного файла](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), добавьте параметр `$select`, включающий только нужные свойства метаданных, исключая свойство **contentBytes**, которое возвращает вложенный файл в формате base64.</span><span class="sxs-lookup"><span data-stu-id="0c18c-184">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-request-get-the-file-attachment-metadata"></a><span data-ttu-id="0c18c-185">Пример запроса: получение метаданных вложенного файла</span><span class="sxs-lookup"><span data-stu-id="0c18c-185">Example request: get the file attachment metadata</span></span>

<span data-ttu-id="0c18c-186">В следующем примере отправитель использует параметр `$select` для получения всех метаданных файла, вложенного в сообщение, кроме свойства **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="0c18c-186">The following example shows the sender using a `$select` parameter to get all the metadata of a file attachment on a message, except **contentBytes**.</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

### <a name="example-response"></a><span data-ttu-id="0c18c-187">Пример отклика</span><span class="sxs-lookup"><span data-stu-id="0c18c-187">Example response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkADI5MAAIT3drCAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "image/jpeg",
    "id": "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=",
    "lastModifiedDateTime": "2019-09-24T23:27:43Z",
    "name": "flower",
    "contentType": "image/jpeg",
    "size": 3640066,
    "isInline": false
}
```

## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="0c18c-188">Альтернатива: отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="0c18c-188">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="0c18c-189">Если необходимо отменить отправку в любое время до окончания срока действия сеанса отправки, можно использовать тот же самый начальный непрозрачный URL-адрес, чтобы удалить сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="0c18c-189">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="0c18c-190">После успешной операции возвращается `HTTP 204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c18c-190">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-request-cancel-an-upload-session"></a><span data-ttu-id="0c18c-191">Пример запроса: отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="0c18c-191">Example request: cancel an upload session</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a><span data-ttu-id="0c18c-192">Пример отклика</span><span class="sxs-lookup"><span data-stu-id="0c18c-192">Example response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a><span data-ttu-id="0c18c-193">Ошибки</span><span class="sxs-lookup"><span data-stu-id="0c18c-193">Errors</span></span>

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a><span data-ttu-id="0c18c-194">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span><span class="sxs-lookup"><span data-stu-id="0c18c-194">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span></span>

<span data-ttu-id="0c18c-195">Эта ошибка возвращается при попытке [создать сеанс отправки](/graph/api/attachment-createuploadsession?view=graph-rest-beta), чтобы вложить файл размером менее 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="0c18c-195">This error is returned when attempting to [create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-beta) to attach a file smaller than 3 MB.</span></span> <span data-ttu-id="0c18c-196">Если размер файла меньше 3 МБ, следует выполнить одну операцию [POST для свойства навигации вложений сообщения](/graph/api/message-post-attachments?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0c18c-196">If the file size is under 3 MB, you should do a single [POST on the attachments navigation property of the message](/graph/api/message-post-attachments?view=graph-rest-beta).</span></span> <span data-ttu-id="0c18c-197">Успешный отклик `POST` включает ИД файла, прикрепленного к сообщению.</span><span class="sxs-lookup"><span data-stu-id="0c18c-197">The successful `POST` response includes the ID of the file attached to the message.</span></span>

