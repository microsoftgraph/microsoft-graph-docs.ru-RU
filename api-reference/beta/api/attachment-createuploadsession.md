---
title: 'вложение: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов файла, чтобы прикрепить файл к указанному сообщению.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116b73b53689c01e346568b6b5d67e56fb31b283
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621619"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="6bfa8-103">вложение: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="6bfa8-103">attachment: createUploadSession</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bfa8-104">Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к указанному [сообщению](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-104">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified [message](../resources/message.md).</span></span>

<span data-ttu-id="6bfa8-105">Используйте этот способ, чтобы вкладывать в **сообщение**файлы размером от 3 МБ до 150MB.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-105">Use this approach to attach files of sizes between 3MB and 150MB to a **message**.</span></span> <span data-ttu-id="6bfa8-106">Чтобы прикрепить файлы размером в 4 МБ, просто [выполните команду POST в свойстве навигации вложений](message-post-attachments.md).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-106">To attach files of sizes under 4MB, simply [POST on the attachments navigation property](message-post-attachments.md).</span></span> 

<span data-ttu-id="6bfa8-107">В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-107">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="6bfa8-108">Заголовки запросов для каждой `PUT` операции позволяют указать точный диапазон байтов для отправки.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-108">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="6bfa8-109">Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-109">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="6bfa8-110">Ниже приведены действия по присоединению файла с помощью сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-110">The following are the steps to attach a file using an upload session:</span></span>

1. <span data-ttu-id="6bfa8-111">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="6bfa8-111">Create an upload session</span></span>
2. <span data-ttu-id="6bfa8-112">В пределах этого сеанса передачи, итеративно отправлять диапазоны байтов (до 4 МБ каждый раз), пока не будут отправлены все байты файла, а файл будет присоединен к указанному сообщению.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-112">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified message</span></span>
3. <span data-ttu-id="6bfa8-113">Сохранение идентификатора вложения для последующего доступа</span><span class="sxs-lookup"><span data-stu-id="6bfa8-113">Save the ID for the attachment for future access</span></span>
4. <span data-ttu-id="6bfa8-114">Необязательно: Удаление сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="6bfa8-114">Optional: Delete the upload session</span></span> 

<span data-ttu-id="6bfa8-115">В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="6bfa8-115">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>


## <a name="permissions"></a><span data-ttu-id="6bfa8-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfa8-116">Permissions</span></span>

<span data-ttu-id="6bfa8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bfa8-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfa8-119">Permission type</span></span>                        | <span data-ttu-id="6bfa8-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6bfa8-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bfa8-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bfa8-122">Mail.ReadWrite</span></span> |
| <span data-ttu-id="6bfa8-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bfa8-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bfa8-124">Mail.ReadWrite</span></span> |
| <span data-ttu-id="6bfa8-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bfa8-125">Application</span></span>                            | <span data-ttu-id="6bfa8-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bfa8-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bfa8-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="6bfa8-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bfa8-128">Request headers</span></span>

| <span data-ttu-id="6bfa8-129">Имя</span><span class="sxs-lookup"><span data-stu-id="6bfa8-129">Name</span></span>          | <span data-ttu-id="6bfa8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6bfa8-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6bfa8-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bfa8-131">Authorization</span></span> | <span data-ttu-id="6bfa8-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6bfa8-132">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="6bfa8-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bfa8-133">Request body</span></span>

<span data-ttu-id="6bfa8-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bfa8-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="6bfa8-135">Parameter</span></span>    | <span data-ttu-id="6bfa8-136">Тип</span><span class="sxs-lookup"><span data-stu-id="6bfa8-136">Type</span></span>        | <span data-ttu-id="6bfa8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="6bfa8-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6bfa8-138">аттачментитем</span><span class="sxs-lookup"><span data-stu-id="6bfa8-138">AttachmentItem</span></span>|[<span data-ttu-id="6bfa8-139">аттачментитем</span><span class="sxs-lookup"><span data-stu-id="6bfa8-139">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="6bfa8-140">Представляет атрибуты элемента, который требуется отправить и вложить.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-140">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="6bfa8-141">Как минимум, укажите тип вложения (`file`), имя и размер файла.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-141">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="6bfa8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-142">Response</span></span>

<span data-ttu-id="6bfa8-143">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-143">If successful, this method returns `201, Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="6bfa8-144">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="6bfa8-144">**Note**:</span></span> 
>
><span data-ttu-id="6bfa8-145">Свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL- `PUT` адресом для последующих запросов на отправку диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-145">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="6bfa8-146">Он содержит соответствующий маркер проверки подлинности `PUT` для последующих запросов, срок действия которых истечет через **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-146">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="6bfa8-147">Не настраивайте этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-147">Do not customize this URL.</span></span>
>
><span data-ttu-id="6bfa8-148">Свойство **nextExpectedRanges** указывает местоположение байта следующего файла, из которого необходимо выполнить загрузку, например `"NextExpectedRanges":["2097152"]`.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-148">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="6bfa8-149">Необходимо отправлять байты в файле по порядку.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-149">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="6bfa8-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="6bfa8-150">Examples</span></span>

<span data-ttu-id="6bfa8-151">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-151">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6bfa8-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-152">Request</span></span>

<span data-ttu-id="6bfa8-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6bfa8-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-154">Response</span></span>

<span data-ttu-id="6bfa8-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-155">The following is an example of the response.</span></span>

> <span data-ttu-id="6bfa8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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