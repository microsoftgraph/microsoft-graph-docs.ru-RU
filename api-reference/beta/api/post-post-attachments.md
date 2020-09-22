---
title: Добавление вложения
description: Добавление вложения при создании записи группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ef75f4b218c84cbb76bfff29d1541a31d29ef530
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014310"
---
# <a name="add-attachment"></a><span data-ttu-id="b42b7-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="b42b7-103">Add attachment</span></span>

<span data-ttu-id="b42b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b42b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b42b7-105">Добавление [вложения](../resources/attachment.md) при создании записи группы.</span><span class="sxs-lookup"><span data-stu-id="b42b7-105">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="b42b7-106">Эта операция ограничит размер вложения, которое можно добавить в течение 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="b42b7-106">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="b42b7-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="b42b7-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="b42b7-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="b42b7-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="b42b7-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="b42b7-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="b42b7-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b42b7-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="b42b7-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b42b7-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b42b7-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b42b7-112">Permissions</span></span>
<span data-ttu-id="b42b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b42b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b42b7-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b42b7-115">Permission type</span></span>      | <span data-ttu-id="b42b7-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b42b7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b42b7-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b42b7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b42b7-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b42b7-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b42b7-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b42b7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b42b7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b42b7-120">Not supported.</span></span>    |
|<span data-ttu-id="b42b7-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b42b7-121">Application</span></span> | <span data-ttu-id="b42b7-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b42b7-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b42b7-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b42b7-123">HTTP request</span></span>
<span data-ttu-id="b42b7-124">Включите вложение при создании [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="b42b7-124">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="b42b7-125">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="b42b7-125">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="b42b7-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b42b7-126">Request headers</span></span>
| <span data-ttu-id="b42b7-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b42b7-127">Header</span></span>       | <span data-ttu-id="b42b7-128">Значение</span><span class="sxs-lookup"><span data-stu-id="b42b7-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b42b7-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b42b7-129">Authorization</span></span>  | <span data-ttu-id="b42b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b42b7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b42b7-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b42b7-132">Request body</span></span>
<span data-ttu-id="b42b7-133">В тексте запроса укажите объект JSON, включающий параметр **POST** .</span><span class="sxs-lookup"><span data-stu-id="b42b7-133">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="b42b7-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="b42b7-134">Parameter</span></span>    | <span data-ttu-id="b42b7-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b42b7-135">Type</span></span>   |<span data-ttu-id="b42b7-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b42b7-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b42b7-137">post</span><span class="sxs-lookup"><span data-stu-id="b42b7-137">post</span></span>|[<span data-ttu-id="b42b7-138">post</span><span class="sxs-lookup"><span data-stu-id="b42b7-138">post</span></span>](../resources/post.md)|<span data-ttu-id="b42b7-139">Новая запись, с которой отправляются ответы, которые включают одно или несколько вложений в коллекцию [вложений](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="b42b7-139">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="b42b7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b42b7-140">Response</span></span>

<span data-ttu-id="b42b7-p104">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="b42b7-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b42b7-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="b42b7-143">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="b42b7-144">Пример 1: включение вложенного файла</span><span class="sxs-lookup"><span data-stu-id="b42b7-144">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="b42b7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b42b7-145">Request</span></span>
<span data-ttu-id="b42b7-146">Ниже приведен пример запроса, включающего файл в качестве вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="b42b7-146">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="http"></a>[<span data-ttu-id="b42b7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b42b7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "Which quarter does that file cover? See my attachment."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.fileAttachment",
      "name": "Another file as attachment",
      "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
    } ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b42b7-148">C#</span><span class="sxs-lookup"><span data-stu-id="b42b7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b42b7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b42b7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b42b7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b42b7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b42b7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b42b7-151">Response</span></span>
<span data-ttu-id="b42b7-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b42b7-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="b42b7-153">Пример 2: включение вложения элемента</span><span class="sxs-lookup"><span data-stu-id="b42b7-153">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="b42b7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="b42b7-154">Request</span></span>
<span data-ttu-id="b42b7-155">Ниже приведен пример запроса, включающего событие в виде вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="b42b7-155">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached an event."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.itemAttachment",
      "name": "Holiday event", 
      "item": {
          "@odata.type": "microsoft.graph.event",
          "subject": "Discuss gifts for children",
          "body": {
              "contentType": "HTML",
              "content": "Let's look for funding!"
          },
          "start": {
              "dateTime": "2019-12-02T18:00:00",
              "timeZone": "Pacific Standard Time"
          },
          "end": {
              "dateTime": "2019-12-02T19:00:00",
              "timeZone": "Pacific Standard Time"
          }
      }
    } ]
  }
}
```


#### <a name="response"></a><span data-ttu-id="b42b7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b42b7-156">Response</span></span>
<span data-ttu-id="b42b7-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b42b7-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="b42b7-158">Пример 3: включение вложения ссылки</span><span class="sxs-lookup"><span data-stu-id="b42b7-158">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="b42b7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b42b7-159">Request</span></span>
<span data-ttu-id="b42b7-160">Ниже приведен пример запроса, включающего вложение ссылки при создании записи.</span><span class="sxs-lookup"><span data-stu-id="b42b7-160">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="b42b7-161">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b42b7-161">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="b42b7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b42b7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached a reference to a file on OneDrive."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.referenceAttachment", 
      "name": "Personal pictures", 
      "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
      "providerType": "oneDriveConsumer", 
      "permission": "Edit", 
      "isFolder": "True"
    } ]
  }
}
```

# <a name="c"></a>[<span data-ttu-id="b42b7-163">C#</span><span class="sxs-lookup"><span data-stu-id="b42b7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b42b7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b42b7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b42b7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b42b7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b42b7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b42b7-166">Response</span></span>
<span data-ttu-id="b42b7-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b42b7-167">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


