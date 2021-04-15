---
title: Отправка документов с помощью API универсальной печати Microsoft Graph
description: Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы Майкрософт.
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: c51d027a0e76f24f6ec4788ae1429adcc29f2948
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766317"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a><span data-ttu-id="d02e2-103">Отправка документов с помощью API универсальной печати Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d02e2-103">Upload documents using the Microsoft Graph Universal Print API</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d02e2-104">Чтобы напечатать документ с помощью API универсальной печати в Microsoft Graph, [создайте задание печати](/graph/api/printershare-post-jobs), отправьте документ и [запустите задание печати](/graph/api/printjob-start).</span><span class="sxs-lookup"><span data-stu-id="d02e2-104">To print a document using the Universal Print API in Microsoft Graph, you [create a print job](/graph/api/printershare-post-jobs), upload a document, and then [start the print job](/graph/api/printjob-start).</span></span> <span data-ttu-id="d02e2-105">В этой статье описано, как отправить документ, начиная с [создания сеанса отправки](/graph/api/printdocument-createuploadsession).</span><span class="sxs-lookup"><span data-stu-id="d02e2-105">This article describes how to upload a document, which starts with [creating an upload session](/graph/api/printdocument-createuploadsession).</span></span>

<span data-ttu-id="d02e2-106">Чтобы отправить файл или его часть, приложение отправляет запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="d02e2-106">To upload a file, or a portion of a file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="d02e2-107">Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером менее 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="d02e2-107">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 10 MB.</span></span>

<span data-ttu-id="d02e2-108">Сегменты файла можно отправлять в любом порядке, в том числе параллельно (до четырех параллельных запросов).</span><span class="sxs-lookup"><span data-stu-id="d02e2-108">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="d02e2-109">После отправки всех двоичных сегментов документа двоичный файл связывается с **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="d02e2-109">When all the binary segments of document are uploaded, the binary file is linked to the **printDocument**.</span></span>

## <a name="http-request"></a><span data-ttu-id="d02e2-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d02e2-110">HTTP request</span></span>

<span data-ttu-id="d02e2-111">Отправьте запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="d02e2-111">Make a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="d02e2-112">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d02e2-112">Request headers</span></span>
| <span data-ttu-id="d02e2-113">Имя</span><span class="sxs-lookup"><span data-stu-id="d02e2-113">Name</span></span>          | <span data-ttu-id="d02e2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d02e2-114">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d02e2-115">Content-Range</span><span class="sxs-lookup"><span data-stu-id="d02e2-115">Content-Range</span></span> | <span data-ttu-id="d02e2-116">Диапазон байтов: {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}.</span><span class="sxs-lookup"><span data-stu-id="d02e2-116">bytes {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}.</span></span> <span data-ttu-id="d02e2-117">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d02e2-117">Required.</span></span>|
| <span data-ttu-id="d02e2-118">Content-Length</span><span class="sxs-lookup"><span data-stu-id="d02e2-118">Content-Length</span></span> | <span data-ttu-id="d02e2-119">{contentLength}‬ обязательно.</span><span class="sxs-lookup"><span data-stu-id="d02e2-119">{contentLength}‬ Required.</span></span>|

### <a name="request-body"></a><span data-ttu-id="d02e2-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d02e2-120">Request body</span></span>
<span data-ttu-id="d02e2-121">Текст запроса — это большой двоичный объект, содержащий байты документа, указанные как **инклюзивный** диапазон байтов, в заголовке `Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="d02e2-121">The request body is a binary blob containing the bytes of the document that are specified as an **inclusive** byte range in the `Content-Range` header.</span></span> 

### <a name="example"></a><span data-ttu-id="d02e2-122">Пример</span><span class="sxs-lookup"><span data-stu-id="d02e2-122">Example</span></span>

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

<span data-ttu-id="d02e2-123">Здесь 0 и 72796 — это индексы начала и окончания сегмента файла, а 4533322 — размер документа.</span><span class="sxs-lookup"><span data-stu-id="d02e2-123">Here, 0 and 72796 are the start and end indexes of the file segment and 4533322 is the size of document.</span></span>
### <a name="http-response"></a><span data-ttu-id="d02e2-124">HTTP-ответ</span><span class="sxs-lookup"><span data-stu-id="d02e2-124">HTTP response</span></span>

<span data-ttu-id="d02e2-125">После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.</span><span class="sxs-lookup"><span data-stu-id="d02e2-125">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

<span data-ttu-id="d02e2-126">С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="d02e2-126">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span> <span data-ttu-id="d02e2-127">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="d02e2-127">You might see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="d02e2-128">Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.</span><span class="sxs-lookup"><span data-stu-id="d02e2-128">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

### <a name="remarks"></a><span data-ttu-id="d02e2-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="d02e2-129">Remarks</span></span>

* <span data-ttu-id="d02e2-p106">При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#get-the-upload-session), чтобы получить более подробный список недостающих диапазонов.</span><span class="sxs-lookup"><span data-stu-id="d02e2-p106">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#get-the-upload-session) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="d02e2-132">В ответ на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`.</span><span class="sxs-lookup"><span data-stu-id="d02e2-132">Including the Authorization header when issuing the `PUT` call might result in a `HTTP 401 Unauthorized` response.</span></span> <span data-ttu-id="d02e2-133">Заголовок авторизации и маркер носителя необходимо отправлять только при создании сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="d02e2-133">The Authorization header and bearer token should only be sent when creating upload session.</span></span> <span data-ttu-id="d02e2-134">Их не следует включать при отправке данных для сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="d02e2-134">It should be not be included when uploading data to upload session.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="d02e2-135">Завершение отправки файла</span><span class="sxs-lookup"><span data-stu-id="d02e2-135">Completing a file</span></span>

<span data-ttu-id="d02e2-136">После получения последнего диапазона байтов файла сервер отправляет ответ `HTTP 201 Created`.</span><span class="sxs-lookup"><span data-stu-id="d02e2-136">When the last byte range of a file is received, the server will response with an `HTTP 201 Created`.</span></span> <span data-ttu-id="d02e2-137">Текст ответа также будет включать набор свойств для связанного **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="d02e2-137">The response body will also include the property set for the associated **printDocument**.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.printDocument", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id": "9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7",
   "documentName": "TestFile.pdf",
   "contentType": "application/pdf", 
   "size": 4533322
}
```

><span data-ttu-id="d02e2-138">**Примечание.** Сеанс отправки удаляется после завершения отправки документов.</span><span class="sxs-lookup"><span data-stu-id="d02e2-138">**Note:** Upload session is deleted after document upload is complete.</span></span>

## <a name="get-the-upload-session"></a><span data-ttu-id="d02e2-139">Получение сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="d02e2-139">Get the upload session</span></span>

<span data-ttu-id="d02e2-140">Чтобы получить сеанс отправки, отправьте запрос GET на URL-адрес отправки.</span><span class="sxs-lookup"><span data-stu-id="d02e2-140">To get upload session, send a GET request to the upload URL.</span></span> 

### <a name="request"></a><span data-ttu-id="d02e2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d02e2-141">Request</span></span>
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="d02e2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02e2-142">Response</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="d02e2-143">Отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="d02e2-143">Cancel the upload session</span></span>

<span data-ttu-id="d02e2-144">Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки.</span><span class="sxs-lookup"><span data-stu-id="d02e2-144">To cancel an upload session, send a DELETE request to the upload URL.</span></span> <span data-ttu-id="d02e2-145">Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).</span><span class="sxs-lookup"><span data-stu-id="d02e2-145">This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="d02e2-146">Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d02e2-146">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="request"></a><span data-ttu-id="d02e2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d02e2-147">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="d02e2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02e2-148">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
