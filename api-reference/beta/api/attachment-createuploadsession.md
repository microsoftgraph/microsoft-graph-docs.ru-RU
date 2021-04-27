---
title: 'вложение: createUploadSession'
description: Создайте сеанс загрузки для итеративных диапазонов загрузки файла, чтобы прикрепить файл к указанному сообщению.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 07b10b2134db7cc8f629a3bef0c6f80ea82d0295
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048038"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="ccb4a-103">вложение: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="ccb4a-103">attachment: createUploadSession</span></span>

<span data-ttu-id="ccb4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccb4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccb4a-105">Создайте сеанс загрузки, который позволяет приложению итеративным образом загружать диапазоны файла, чтобы прикрепить файл к элементу Outlook.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.</span></span> <span data-ttu-id="ccb4a-106">Элемент может быть [сообщением или](../resources/message.md) [событием.](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="ccb4a-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="ccb4a-107">Используйте этот подход, чтобы прикрепить файл, если размер файла составляет от 3 до 150 МБ.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="ccb4a-108">Чтобы прикрепить файл размером менее 3 МБ, необходимо сделать операцию по свойству навигации вложения элемента Outlook; узнайте, как это сделать для сообщения или `POST` события.  [](message-post-attachments.md) [](event-post-attachments.md)</span><span class="sxs-lookup"><span data-stu-id="ccb4a-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="ccb4a-109">В рамках ответа это действие возвращает URL-адрес загрузки, который можно использовать в последующих последовательном `PUT` запросах.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="ccb4a-110">Запросить заглавные главы для каждой операции, чтобы указать точный диапазон отгрузки `PUT` bytes.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="ccb4a-111">Это позволяет возобновить передачу, если подключение к сети будет отброшено во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="ccb4a-112">Ниже положены действия по присоединению файла к элементу Outlook с помощью сеанса загрузки:</span><span class="sxs-lookup"><span data-stu-id="ccb4a-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="ccb4a-113">Создание сеанса загрузки.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-113">Create an upload session.</span></span>
2. <span data-ttu-id="ccb4a-114">В течение этого сеанса загрузки итеративным образом загружаются диапазоны bytes (до 4 МБ каждый раз), пока не будут загружены все bytes файла и файл присоединен к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="ccb4a-115">Сохраните ID для вложения для будущего доступа.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="ccb4a-116">Необязательный. Удалите сеанс загрузки.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="ccb4a-117">См. в примере Outlook большие файлы [для сообщений](/graph/outlook-large-attachments) или событий.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="ccb4a-118">Exchange Online позволяет администраторам настраивать ограничение размера сообщения для Microsoft 365 почтовых ящиков, включая любые вложения сообщений.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-118">Exchange Online lets administrators customize the message size limit for Microsoft 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="ccb4a-119">По умолчанию это ограничение размера сообщения — 35 МБ.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="ccb4a-120">Узнайте, как [настроить максимальный](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) размер сообщения для поддержки вложений, которые больше, чем по умолчанию для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="ccb4a-121">При [присоединении](/graph/known-issues#attaching-large-files-to-messages) большого файла к сообщению или событию в общем или делегированного почтовом ящике следует помнить о известной проблеме.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>


## <a name="permissions"></a><span data-ttu-id="ccb4a-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccb4a-122">Permissions</span></span>

<span data-ttu-id="ccb4a-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccb4a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccb4a-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccb4a-125">Permission type</span></span>                        | <span data-ttu-id="ccb4a-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccb4a-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ccb4a-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccb4a-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccb4a-128">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccb4a-128">Mail.ReadWrite</span></span> |
| <span data-ttu-id="ccb4a-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccb4a-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccb4a-130">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccb4a-130">Mail.ReadWrite</span></span> |
| <span data-ttu-id="ccb4a-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccb4a-131">Application</span></span>                            | <span data-ttu-id="ccb4a-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccb4a-132">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccb4a-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccb4a-133">HTTP request</span></span>

<span data-ttu-id="ccb4a-134">Создание сеанса загрузки для прикрепления файла к **событию:**</span><span class="sxs-lookup"><span data-stu-id="ccb4a-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="ccb4a-135">Создание сеанса загрузки для прикрепления файла к **сообщению:**</span><span class="sxs-lookup"><span data-stu-id="ccb4a-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="ccb4a-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccb4a-136">Request headers</span></span>

| <span data-ttu-id="ccb4a-137">Имя</span><span class="sxs-lookup"><span data-stu-id="ccb4a-137">Name</span></span>          | <span data-ttu-id="ccb4a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ccb4a-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ccb4a-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccb4a-139">Authorization</span></span> | <span data-ttu-id="ccb4a-140">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ccb4a-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="ccb4a-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccb4a-141">Request body</span></span>

<span data-ttu-id="ccb4a-142">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccb4a-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="ccb4a-143">Parameter</span></span>    | <span data-ttu-id="ccb4a-144">Тип</span><span class="sxs-lookup"><span data-stu-id="ccb4a-144">Type</span></span>        | <span data-ttu-id="ccb4a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ccb4a-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ccb4a-146">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="ccb4a-146">AttachmentItem</span></span>|[<span data-ttu-id="ccb4a-147">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="ccb4a-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="ccb4a-148">Представляет атрибуты элемента, который будет загружен и присоединен.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="ccb4a-149">Как минимум укажите тип вложения `file` (), имя и размер файла.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="ccb4a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccb4a-150">Response</span></span>

<span data-ttu-id="ccb4a-151">В случае успешной работы этот метод возвращает код ответа и новый объект `201 Created` [uploadSession](../resources/uploadsession.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="ccb4a-152">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="ccb4a-152">**Note**:</span></span> 
>
><span data-ttu-id="ccb4a-153">Свойство **uploadUrl,** возвращенное в рамках объекта ответа **uploadSession,** является непрозрачной URL-адресом для последующих запросов для загрузки байт-диапазонов `PUT` файла.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="ccb4a-154">Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действияDateTime.**</span><span class="sxs-lookup"><span data-stu-id="ccb4a-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="ccb4a-155">Не настраивать этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="ccb4a-156">Свойство **nextExpectedRanges** указывает следующее расположение byte файла, чтобы загрузить из, например, `"NextExpectedRanges":["2097152"]` .</span><span class="sxs-lookup"><span data-stu-id="ccb4a-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="ccb4a-157">Байты файла необходимо отправлять по порядку.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="ccb4a-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="ccb4a-158">Examples</span></span>

<span data-ttu-id="ccb4a-159">В следующем примере показано, как создать сеанс загрузки, который можно использовать в последующих операциях по отправке файлов в указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="ccb4a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccb4a-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccb4a-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccb4a-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ccb4a-162">C#</span><span class="sxs-lookup"><span data-stu-id="ccb4a-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccb4a-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccb4a-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccb4a-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccb4a-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccb4a-165">Java</span><span class="sxs-lookup"><span data-stu-id="ccb4a-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccb4a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccb4a-166">Response</span></span>

> <span data-ttu-id="ccb4a-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ccb4a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


