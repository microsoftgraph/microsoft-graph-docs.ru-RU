---
title: Вложение крупных файлов в сообщения и события Outlook
description: В зависимости от размера файла можно выбрать один из двух способов вложения файлов в сообщения или события.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 30589b4aeeb6d6f8a17dfefd677abadeba3c76bd
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590916"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a><span data-ttu-id="e6af6-103">Вложение крупных файлов в сообщения и события Outlook</span><span class="sxs-lookup"><span data-stu-id="e6af6-103">Attach large files to Outlook messages or events</span></span>

<span data-ttu-id="e6af6-104">С помощью API Microsoft Graph можно вкладывать файлы размером до 150 МБ в элементы Outlook [сообщение](/graph/api/resources/message?view=graph-rest-1.0) или [событие](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e6af6-104">Using the Microsoft Graph API, you can attach files up to 150 MB to an Outlook [message](/graph/api/resources/message?view=graph-rest-1.0) or [event](/graph/api/resources/event?view=graph-rest-1.0) item.</span></span> <span data-ttu-id="e6af6-105">В зависимости от размера файла выберите один из двух способов вложения файла:</span><span class="sxs-lookup"><span data-stu-id="e6af6-105">Depending on the file size, choose one of two ways to attach the file:</span></span>
- <span data-ttu-id="e6af6-106">Если размер файла не превышает 3 МБ, выполните одну операцию POST в свойстве навигации **attachments** элемента Outlook. Узнайте, как это выполняется [для сообщения](/graph/api/message-post-attachments?view=graph-rest-1.0) или [события](/graph/api/event-post-attachments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e6af6-106">If the file size is under 3 MB, do a single POST on the **attachments** navigation property of the Outlook item; see how to do this [for a message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [for an event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="e6af6-107">Успешный отклик `POST` включает ИД вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="e6af6-107">The successful `POST` response includes the ID of the file attachment.</span></span>
- <span data-ttu-id="e6af6-108">Если размер файла составляет от 3 до 150 МБ, создайте сеанс отправки и итеративно используйте `PUT` для отправки диапазонов байтов, пока не будет отправлен весь файл.</span><span class="sxs-lookup"><span data-stu-id="e6af6-108">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="e6af6-109">Заголовок в итоговом успешном отклике `PUT` включает URL-адрес с ИД вложения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-109">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span>

<span data-ttu-id="e6af6-110">Чтобы вложить в сообщение несколько файлов, выберите способ для каждого файла на основе их размеров и вложите файлы по отдельности.</span><span class="sxs-lookup"><span data-stu-id="e6af6-110">To attach multiple files to a message, choose the approach for each file based on its file size and attach the files individually.</span></span>

<span data-ttu-id="e6af6-111">В этой статье пошагово демонстрируется второй подход с созданием и использованием сеанса отправки для добавления большого вложенного файла (размером более 3 МБ) в элемент Outlook.</span><span class="sxs-lookup"><span data-stu-id="e6af6-111">This article illustrates the second approach step by step, creating and using an upload session to add a large file attachment (of size over 3MB) to an Outlook item.</span></span> <span data-ttu-id="e6af6-112">На каждом шаге демонстрируется соответствующий код для сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="e6af6-112">Each step shows the corresponding code for a message and for an event.</span></span> <span data-ttu-id="e6af6-113">После успешной отправки целого файла в статье показано получение заголовка отклика, содержащего идентификатор вложения файла, который затем используется для получения необработанного содержимого или метаданных вложения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-113">Upon successfully uploading the entire file, the article shows getting a response header that contains an ID for the file attachment, and then using that attachment ID to get the raw attachment content or attachment metadata.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="e6af6-114">Обратите внимание на [известную проблему](known-issues.md#attaching-large-files-to-messages) при вложении больших файлов в сообщение или событие в общем или делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e6af6-114">Be aware of a [known issue](known-issues.md#attaching-large-files-to-messages) if you're attaching large files to a message or event in a shared or delegated mailbox.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="e6af6-115">Шаг 1. Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="e6af6-115">Step 1: Create an upload session</span></span>

<span data-ttu-id="e6af6-116">[Создайте сеанс отправки](/graph/api/attachment-createuploadsession?view=graph-rest-1.0), чтобы вложить файл в сообщение или событие.</span><span class="sxs-lookup"><span data-stu-id="e6af6-116">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file to a message or event.</span></span> <span data-ttu-id="e6af6-117">Укажите файл во входном параметре **AttachmentItem**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-117">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="e6af6-118">После успешной операции возвращается `HTTP 201 Created` и новый экземпляр объекта [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0), содержащий непрозрачный URL-адрес, который можно использовать в последующих операциях `PUT` для отправки частей этого файла.</span><span class="sxs-lookup"><span data-stu-id="e6af6-118">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="e6af6-119">Этот экземпляр **uploadSession** предоставляет временное место хранения, где байты файла сохраняются до отправки всего файла.</span><span class="sxs-lookup"><span data-stu-id="e6af6-119">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="e6af6-120">Обязательно запросите разрешение `Mail.ReadWrite` на создание экземпляра **uploadSession** для сообщения и экземпляра `Calendars.ReadWrite` для события.</span><span class="sxs-lookup"><span data-stu-id="e6af6-120">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession** for a message, and `Calendars.ReadWrite` for an event.</span></span> <span data-ttu-id="e6af6-121">Непрозрачный URL-адрес, возвращенный свойством **uploadUrl** нового объекта **uploadSession**, проходит предварительную проверку подлинности и содержит соответствующий маркер авторизации для последующих запросов `PUT` в домене `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-121">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="e6af6-122">Этот маркер истекает в срок **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-122">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="e6af6-123">Не следует изменять этот URL-адрес для операций `PUT`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-123">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="e6af6-124">Объект **uploadSession** в отклике также включает свойство **nextExpectedRanges**, указывающее, что начальное место отправки должно быть байтом 0.</span><span class="sxs-lookup"><span data-stu-id="e6af6-124">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-create-an-upload-session-for-a-message"></a><span data-ttu-id="e6af6-125">Пример: создание сеанса отправки для сообщения</span><span class="sxs-lookup"><span data-stu-id="e6af6-125">Example: create an upload session for a message</span></span>

#### <a name="request"></a><span data-ttu-id="e6af6-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-126">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e6af6-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6af6-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_message",
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
# <a name="c"></a>[<span data-ttu-id="e6af6-128">C#</span><span class="sxs-lookup"><span data-stu-id="e6af6-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6af6-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6af6-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6af6-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6af6-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e6af6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-131">Response</span></span>
<span data-ttu-id="e6af6-132">В следующем примере отклика демонстрируется ресурс **uploadSession**, возвращаемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-132">The following example response shows the **uploadSession** resource returned for the message.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_message",
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

### <a name="example-create-an-upload-session-for-an-event"></a><span data-ttu-id="e6af6-133">Пример: создание сеанса отправки для события</span><span class="sxs-lookup"><span data-stu-id="e6af6-133">Example: create an upload session for an event</span></span>
#### <a name="request"></a><span data-ttu-id="e6af6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-134">Request</span></span> 

<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_event",
  "sampleKeys": ["AAMkADU5CCmSAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```


#### <a name="response"></a><span data-ttu-id="e6af6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-135">Response</span></span>
<span data-ttu-id="e6af6-136">В следующем примере отклика демонстрируется ресурс **uploadSession**, возвращаемый для события.</span><span class="sxs-lookup"><span data-stu-id="e6af6-136">The following example response shows the **uploadSession** resource returned for the event.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw",
    "expirationDateTime": "2020-02-22T02:46:56.7410786Z",
    "nextExpectedRanges": [
        "0-"
    ]
}

```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="e6af6-137">Шаг 2. Отправка диапазона байтов файла с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="e6af6-137">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="e6af6-138">Чтобы отправить файл или часть файла, выполните запрос `PUT` к URL-адресу, возвращенному на шаге 1 в свойстве **uploadUrl** ресурса **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-138">To upload the file, or a portion of the file, make a `PUT` request to the URL returned in step 1 in the **uploadUrl** property of the **uploadSession** resource.</span></span> <span data-ttu-id="e6af6-139">Можно отправить файл целиком или разделить файл на несколько диапазонов байтов.</span><span class="sxs-lookup"><span data-stu-id="e6af6-139">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="e6af6-140">Для более высокой производительности размер каждого диапазона байтов не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="e6af6-140">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="e6af6-141">Укажите заголовки и основной текст запроса, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="e6af6-141">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="e6af6-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6af6-142">Request headers</span></span>

| <span data-ttu-id="e6af6-143">Имя</span><span class="sxs-lookup"><span data-stu-id="e6af6-143">Name</span></span>       | <span data-ttu-id="e6af6-144">Тип</span><span class="sxs-lookup"><span data-stu-id="e6af6-144">Type</span></span> | <span data-ttu-id="e6af6-145">Описание</span><span class="sxs-lookup"><span data-stu-id="e6af6-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6af6-146">Content-Length</span><span class="sxs-lookup"><span data-stu-id="e6af6-146">Content-Length</span></span> | <span data-ttu-id="e6af6-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af6-147">Int32</span></span> | <span data-ttu-id="e6af6-148">Количество байтов, отправляемых в этой операции.</span><span class="sxs-lookup"><span data-stu-id="e6af6-148">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="e6af6-149">Для более высокой производительности количество байт в каждой операции `PUT` не должно превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="e6af6-149">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="e6af6-150">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e6af6-150">Required.</span></span> |
| <span data-ttu-id="e6af6-151">Content-Range</span><span class="sxs-lookup"><span data-stu-id="e6af6-151">Content-Range</span></span> | <span data-ttu-id="e6af6-152">String</span><span class="sxs-lookup"><span data-stu-id="e6af6-152">String</span></span> | <span data-ttu-id="e6af6-153">Диапазон байтов файла, отправляемого в этой операции, начиная с байта 0, выраженный в формате `bytes {start}-{end}/{total}`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-153">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="e6af6-154">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e6af6-154">Required.</span></span> |
| <span data-ttu-id="e6af6-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6af6-155">Content-Type</span></span> | <span data-ttu-id="e6af6-156">String</span><span class="sxs-lookup"><span data-stu-id="e6af6-156">String</span></span>  | <span data-ttu-id="e6af6-157">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="e6af6-157">The MIME type.</span></span> <span data-ttu-id="e6af6-158">Укажите `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-158">Specify `application/octet-stream`.</span></span> <span data-ttu-id="e6af6-159">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e6af6-159">Required.</span></span> |

<span data-ttu-id="e6af6-160">Не указывайте заголовок запроса `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-160">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="e6af6-161">Запрос `PUT` использует прошедший предварительную проверку подлинности URL-адрес из свойства **uploadUrl**, что позволяет получить доступ к домену `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-161">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="e6af6-162">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6af6-162">Request body</span></span>

<span data-ttu-id="e6af6-163">Укажите фактические байты вкладываемого файла, находящиеся в диапазоне расположения, указанном в заголовке запроса `Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-163">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="e6af6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-164">Response</span></span>
<span data-ttu-id="e6af6-165">После успешной отправки возвращается `HTTP 200 OK` и объект **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-165">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="e6af6-166">Объект отклика имеет указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="e6af6-166">Note the following in the response object:</span></span>

- <span data-ttu-id="e6af6-167">Свойство **ExpirationDateTime** указывает дату и время окончания срока действия для маркера авторизации, внедренного в значение свойства **uploadUrl**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-167">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="e6af6-168">Это значение даты и времени окончания срока действия остается таким же, какое было возвращено начальным объектом **uploadSession** на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="e6af6-168">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="e6af6-169">Свойство **NextExpectedRanges** указывает расположение следующего байта, с которого необходимо начать отправку, например `"NextExpectedRanges":["2097152"]`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-169">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="e6af6-170">Байты файла необходимо отправлять по порядку.</span><span class="sxs-lookup"><span data-stu-id="e6af6-170">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="e6af6-171">Свойство **uploadUrl** не возвращается явным образом, поскольку все операции `PUT` сеанса отправки используют тот же самый URL-адрес, который был возвращен при создании сеанса (на шаге 1).</span><span class="sxs-lookup"><span data-stu-id="e6af6-171">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-first-upload-to-the-message"></a><span data-ttu-id="e6af6-172">Пример: первая отправка в сообщение</span><span class="sxs-lookup"><span data-stu-id="e6af6-172">Example: first upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="e6af6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-173">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="e6af6-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-174">Response</span></span>

<span data-ttu-id="e6af6-175">В следующем примере отклика в свойстве **NextExpectedRanges** демонстрируется начало следующего диапазона байтов, ожидаемого сервером.</span><span class="sxs-lookup"><span data-stu-id="e6af6-175">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
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

### <a name="example-first-upload-to-the-event"></a><span data-ttu-id="e6af6-176">Пример: первая отправка в событие</span><span class="sxs-lookup"><span data-stu-id="e6af6-176">Example: first upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="e6af6-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-177">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="e6af6-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-178">Response</span></span>

<span data-ttu-id="e6af6-179">В следующем примере отклика в свойстве **NextExpectedRanges** демонстрируется начало следующего диапазона байтов, ожидаемого сервером.</span><span class="sxs-lookup"><span data-stu-id="e6af6-179">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69%4098a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA%3D')/AttachmentSessions/$entity",
    "ExpirationDateTime":"2020-02-22T02:46:56.7410786Z",
    "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="e6af6-180">Шаг 3. Продолжение отправки диапазонов байтов вплоть до отправки всего файла</span><span class="sxs-lookup"><span data-stu-id="e6af6-180">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="e6af6-181">После первоначальной отправки на шаге 2 продолжайте отправлять оставшиеся части файла, используя аналогичный запрос `PUT`, как описано на шаге 2, до достижения даты и времени окончания срока действия сеанса.</span><span class="sxs-lookup"><span data-stu-id="e6af6-181">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="e6af6-182">Получайте значение **NextExpectedRanges**, чтобы определить, с какого места должен начинаться следующий диапазон байтов для отправки.</span><span class="sxs-lookup"><span data-stu-id="e6af6-182">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="e6af6-183">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="e6af6-183">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="e6af6-184">Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="e6af6-184">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="e6af6-185">После успешной отправки последнего байта файла операция `PUT` возвращает `HTTP 201 Created` и заголовок `Location`, указывающий URL-адрес вложенного файла в домене `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-185">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="e6af6-186">Можно получить ИД вложения по этому URL-адресу и сохранить его для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="e6af6-186">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="e6af6-187">В зависимости от сценария можно использовать этот ИД для [получения метаданных вложения](/graph/api/attachment-get?view=graph-rest-1.0) или для [удаления вложения из элемента Outlook](/graph/api/attachment-delete?view=graph-rest-1.0) с помощью конечной точки Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e6af6-187">Depending on your scenario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-1.0), or [remove the attachment from the Outlook item](/graph/api/attachment-delete?view=graph-rest-1.0) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="e6af6-188">В следующих примерах показана отправка последнего диапазона байтов файла в сообщение и событие из предыдущих шагов.</span><span class="sxs-lookup"><span data-stu-id="e6af6-188">The following examples show uploading the last byte range of the file to the message and to the event in the preceding steps.</span></span>

### <a name="example-final-upload-to-the-message"></a><span data-ttu-id="e6af6-189">Пример: окончательная отправка в сообщение</span><span class="sxs-lookup"><span data-stu-id="e6af6-189">Example: final upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="e6af6-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-190">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="e6af6-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-191">Response</span></span>
<span data-ttu-id="e6af6-192">В следующем примере отклика показан заголовок отклика `Location`, из которого можно сохранить идентификатор вложения (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) для дальнейшего применения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-192">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a><span data-ttu-id="e6af6-193">Пример: окончательная отправка в событие</span><span class="sxs-lookup"><span data-stu-id="e6af6-193">Example: final upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="e6af6-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-194">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="e6af6-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-195">Response</span></span>
<span data-ttu-id="e6af6-196">В следующем примере отклика показан заголовок отклика `Location`, из которого можно сохранить идентификатор вложения (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) для дальнейшего применения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-196">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a><span data-ttu-id="e6af6-197">Шаг 4 (необязательно). Получение вложенного файла из элемента Outlook</span><span class="sxs-lookup"><span data-stu-id="e6af6-197">Step 4 (optional): Get the file attachment from the Outlook item</span></span>

<span data-ttu-id="e6af6-198">Как всегда, при [получении вложения](/graph/api/attachment-get?view=graph-rest-1.0) из элемента Outlook размер вложения не ограничивается технически.</span><span class="sxs-lookup"><span data-stu-id="e6af6-198">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-1.0) from an Outlook item is not technically limited by attachment size.</span></span>

<span data-ttu-id="e6af6-199">Тем не менее, получение большого вложенного файла в формате кодировки base64 влияет на производительность API.</span><span class="sxs-lookup"><span data-stu-id="e6af6-199">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="e6af6-200">Если ожидается вложение большого размера:</span><span class="sxs-lookup"><span data-stu-id="e6af6-200">If you expect a large attachment:</span></span>

- <span data-ttu-id="e6af6-201">Вместо получения вложенного содержимого в формате base64 можно [получить необработанные данные вложенного файла](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="e6af6-201">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>
- <span data-ttu-id="e6af6-202">Чтобы [получить метаданные вложенного файла](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment), добавьте параметр `$select`, включающий только нужные свойства метаданных, исключая свойство **contentBytes**, которое возвращает вложенный файл в формате base64.</span><span class="sxs-lookup"><span data-stu-id="e6af6-202">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-get-the-raw-file-attached-to-the-event"></a><span data-ttu-id="e6af6-203">Пример: получение необработанного файла, вложенного в событие</span><span class="sxs-lookup"><span data-stu-id="e6af6-203">Example: Get the raw file attached to the event</span></span>
<span data-ttu-id="e6af6-204">После примера события и использования идентификатора вложения, возвращаемого в заголовке `Location` предыдущего шага, в следующем примере запроса демонстрируется использование параметра `$value` для получения необработанных данных содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="e6af6-204">Following the event example and using the attachment ID returned in the `Location` header of the previous step, the next example request shows using a `$value` parameter to get the attachment raw content data.</span></span>

#### <a name="request"></a><span data-ttu-id="e6af6-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-205">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a><span data-ttu-id="e6af6-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-206">Response</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
content-length: 3483322
Content-type: image/jpeg

{Raw bytes of the file}
```


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a><span data-ttu-id="e6af6-207">Пример: получение метаданных файла, вложенного в сообщение</span><span class="sxs-lookup"><span data-stu-id="e6af6-207">Example: Get the metadata of the file attached to the message</span></span>
<span data-ttu-id="e6af6-208">После примера сообщения в следующем примере запроса демонстрируется использование параметра `$select` для получения некоторых метаданных файла, вложенного в сообщение, кроме **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="e6af6-208">Following the message example, the next example request shows using a `$select` parameter to get some of the metadata of a file attachment on a message, excluding **contentBytes**.</span></span>

#### <a name="request"></a><span data-ttu-id="e6af6-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-209">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a><span data-ttu-id="e6af6-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-210">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment_metadata",
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


## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="e6af6-211">Альтернатива: отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="e6af6-211">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="e6af6-212">Если необходимо отменить отправку в любое время до окончания срока действия сеанса отправки, можно использовать тот же самый начальный непрозрачный URL-адрес, чтобы удалить сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="e6af6-212">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="e6af6-213">После успешной операции возвращается `HTTP 204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6af6-213">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-cancel-the-upload-session-for-the-message"></a><span data-ttu-id="e6af6-214">Пример: отмена сеанса отправки для сообщения</span><span class="sxs-lookup"><span data-stu-id="e6af6-214">Example: cancel the upload session for the message</span></span>

#### <a name="request"></a><span data-ttu-id="e6af6-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6af6-215">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a><span data-ttu-id="e6af6-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6af6-216">Response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a><span data-ttu-id="e6af6-217">Ошибки</span><span class="sxs-lookup"><span data-stu-id="e6af6-217">Errors</span></span>

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a><span data-ttu-id="e6af6-218">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span><span class="sxs-lookup"><span data-stu-id="e6af6-218">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span></span>

<span data-ttu-id="e6af6-219">Эта ошибка возвращается при попытке [создать сеанс отправки](/graph/api/attachment-createuploadsession?view=graph-rest-1.0), чтобы вложить файл размером менее 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="e6af6-219">This error is returned when attempting to [create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file smaller than 3 MB.</span></span> <span data-ttu-id="e6af6-220">Если размер файла меньше 3 МБ, следует выполнить одну операцию POST для свойства навигации **attachments** [сообщения](/graph/api/message-post-attachments?view=graph-rest-1.0) или [события](/graph/api/event-post-attachments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e6af6-220">If the file size is under 3 MB, you should do a single POST on the **attachments** navigation property [of the message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [of the event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="e6af6-221">Успешный отклик `POST` включает ИД файла, прикрепленного к сообщению.</span><span class="sxs-lookup"><span data-stu-id="e6af6-221">The successful `POST` response includes the ID of the file attached to the message.</span></span>

