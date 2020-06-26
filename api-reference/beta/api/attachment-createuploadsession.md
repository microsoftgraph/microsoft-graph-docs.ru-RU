---
title: 'вложение: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов файла, чтобы прикрепить файл к указанному сообщению.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c06699c99a381e46195f9e9bcb4eb772655df349
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895701"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="71cc8-103">вложение: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="71cc8-103">attachment: createUploadSession</span></span>

<span data-ttu-id="71cc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71cc8-105">Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к элементу Outlook.</span><span class="sxs-lookup"><span data-stu-id="71cc8-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.</span></span> <span data-ttu-id="71cc8-106">Элемент может быть [сообщением](../resources/message.md) или [событием](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="71cc8-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="71cc8-107">Используйте этот способ, чтобы вложить файл, если размер файла находится в пределах от 3 МБ до 150 МБ.</span><span class="sxs-lookup"><span data-stu-id="71cc8-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="71cc8-108">Чтобы присоединить файл размером менее 3 МБ, выполните `POST` операцию над свойством навигации **вложений** элемента Outlook, чтобы узнать, как это сделать [для сообщения](message-post-attachments.md) или [для события](event-post-attachments.md).</span><span class="sxs-lookup"><span data-stu-id="71cc8-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="71cc8-109">В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах.</span><span class="sxs-lookup"><span data-stu-id="71cc8-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="71cc8-110">Заголовки запросов для каждой `PUT` операции позволяют указать точный диапазон байтов для отправки.</span><span class="sxs-lookup"><span data-stu-id="71cc8-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="71cc8-111">Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки.</span><span class="sxs-lookup"><span data-stu-id="71cc8-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="71cc8-112">Ниже приведены действия по присоединению файла к элементу Outlook с помощью сеанса отправки:</span><span class="sxs-lookup"><span data-stu-id="71cc8-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="71cc8-113">Создание сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="71cc8-113">Create an upload session.</span></span>
2. <span data-ttu-id="71cc8-114">В пределах этого сеанса передачи, итеративно отправлять диапазоны байтов (до 4 МБ каждый раз), пока не будут отправлены все байты файла, а файл будет присоединен к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="71cc8-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="71cc8-115">Сохраните идентификатор вложения для последующего доступа.</span><span class="sxs-lookup"><span data-stu-id="71cc8-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="71cc8-116">Необязательно: удалите сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="71cc8-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="71cc8-117">В этом примере показано, [как прикрепить крупные файлы к сообщениям или событиям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="71cc8-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="71cc8-118">Exchange Online позволяет администраторам настраивать ограничения на размер сообщений для почтовых ящиков Microsoft 365, включая вложения сообщений.</span><span class="sxs-lookup"><span data-stu-id="71cc8-118">Exchange Online lets administrators customize the message size limit for Microsoft 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="71cc8-119">По умолчанию это максимальный размер сообщения 35 МБ.</span><span class="sxs-lookup"><span data-stu-id="71cc8-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="71cc8-120">Узнайте [, как настроить максимальный размер сообщения](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) для поддержки вложений, превышающих ограничение по умолчанию для клиента.</span><span class="sxs-lookup"><span data-stu-id="71cc8-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="71cc8-121">Если вы присоединяете большой файл к сообщению или событию в общем или делегированном почтовом ящике, учитывайте [известную ошибку](/graph/known-issues#attaching-large-files-to-messages) .</span><span class="sxs-lookup"><span data-stu-id="71cc8-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>


## <a name="permissions"></a><span data-ttu-id="71cc8-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71cc8-122">Permissions</span></span>

<span data-ttu-id="71cc8-123">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="71cc8-123">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="71cc8-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71cc8-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71cc8-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71cc8-125">Permission type</span></span>                        | <span data-ttu-id="71cc8-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71cc8-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71cc8-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71cc8-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="71cc8-128">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71cc8-128">Mail.ReadWrite</span></span> |
| <span data-ttu-id="71cc8-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71cc8-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cc8-130">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71cc8-130">Mail.ReadWrite</span></span> |
| <span data-ttu-id="71cc8-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71cc8-131">Application</span></span>                            | <span data-ttu-id="71cc8-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71cc8-132">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71cc8-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71cc8-133">HTTP request</span></span>

<span data-ttu-id="71cc8-134">Создание сеанса отправки для присоединения файла к **событию**:</span><span class="sxs-lookup"><span data-stu-id="71cc8-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="71cc8-135">Создание сеанса отправки для вложения файла в **сообщение**:</span><span class="sxs-lookup"><span data-stu-id="71cc8-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="71cc8-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71cc8-136">Request headers</span></span>

| <span data-ttu-id="71cc8-137">Имя</span><span class="sxs-lookup"><span data-stu-id="71cc8-137">Name</span></span>          | <span data-ttu-id="71cc8-138">Описание</span><span class="sxs-lookup"><span data-stu-id="71cc8-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="71cc8-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71cc8-139">Authorization</span></span> | <span data-ttu-id="71cc8-140">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="71cc8-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="71cc8-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71cc8-141">Request body</span></span>

<span data-ttu-id="71cc8-142">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="71cc8-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71cc8-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="71cc8-143">Parameter</span></span>    | <span data-ttu-id="71cc8-144">Тип</span><span class="sxs-lookup"><span data-stu-id="71cc8-144">Type</span></span>        | <span data-ttu-id="71cc8-145">Описание</span><span class="sxs-lookup"><span data-stu-id="71cc8-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71cc8-146">аттачментитем</span><span class="sxs-lookup"><span data-stu-id="71cc8-146">AttachmentItem</span></span>|[<span data-ttu-id="71cc8-147">аттачментитем</span><span class="sxs-lookup"><span data-stu-id="71cc8-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="71cc8-148">Представляет атрибуты элемента, который требуется отправить и вложить.</span><span class="sxs-lookup"><span data-stu-id="71cc8-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="71cc8-149">Как минимум, укажите тип вложения ( `file` ), имя и размер файла.</span><span class="sxs-lookup"><span data-stu-id="71cc8-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="71cc8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="71cc8-150">Response</span></span>

<span data-ttu-id="71cc8-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71cc8-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="71cc8-152">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="71cc8-152">**Note**:</span></span> 
>
><span data-ttu-id="71cc8-153">Свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL-адресом для последующих `PUT` запросов на отправку диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="71cc8-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="71cc8-154">Он содержит соответствующий маркер проверки подлинности для последующих `PUT` запросов, срок действия которых истечет через **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="71cc8-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="71cc8-155">Не настраивайте этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="71cc8-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="71cc8-156">Свойство **nextExpectedRanges** указывает местоположение байта следующего файла, из которого необходимо выполнить загрузку, например `"NextExpectedRanges":["2097152"]` .</span><span class="sxs-lookup"><span data-stu-id="71cc8-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="71cc8-157">Байты файла необходимо отправлять по порядку.</span><span class="sxs-lookup"><span data-stu-id="71cc8-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="71cc8-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="71cc8-158">Examples</span></span>

<span data-ttu-id="71cc8-159">В приведенном ниже примере показано, как создать сеанс отправки, который можно использовать в последующих операциях отправки файлов для указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="71cc8-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="71cc8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="71cc8-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="71cc8-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="71cc8-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
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
# <a name="c"></a>[<span data-ttu-id="71cc8-162">C#</span><span class="sxs-lookup"><span data-stu-id="71cc8-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71cc8-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71cc8-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71cc8-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71cc8-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71cc8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="71cc8-165">Response</span></span>

> <span data-ttu-id="71cc8-166">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="71cc8-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="71cc8-167">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="71cc8-167">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
