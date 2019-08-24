---
title: Добавление вложения
description: Добавление вложения при создании записи группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e82f7d7cc7a0ceaac437cb86020ad62bc470b3e1
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622589"
---
# <a name="add-attachment"></a><span data-ttu-id="74e64-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="74e64-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e64-104">Добавление [вложения](../resources/attachment.md) при создании записи группы.</span><span class="sxs-lookup"><span data-stu-id="74e64-104">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="74e64-105">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="74e64-105">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="74e64-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="74e64-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="74e64-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="74e64-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="74e64-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="74e64-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="74e64-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="74e64-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="74e64-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="74e64-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="74e64-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74e64-111">Permissions</span></span>
<span data-ttu-id="74e64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e64-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74e64-114">Permission type</span></span>      | <span data-ttu-id="74e64-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74e64-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e64-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74e64-116">Delegated (work or school account)</span></span> | <span data-ttu-id="74e64-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e64-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74e64-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74e64-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e64-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e64-119">Not supported.</span></span>    |
|<span data-ttu-id="74e64-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74e64-120">Application</span></span> | <span data-ttu-id="74e64-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e64-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e64-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74e64-122">HTTP request</span></span>
<span data-ttu-id="74e64-123">Включите вложение при создании [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="74e64-123">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="74e64-124">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="74e64-124">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="74e64-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74e64-125">Request headers</span></span>
| <span data-ttu-id="74e64-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74e64-126">Header</span></span>       | <span data-ttu-id="74e64-127">Значение</span><span class="sxs-lookup"><span data-stu-id="74e64-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74e64-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74e64-128">Authorization</span></span>  | <span data-ttu-id="74e64-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74e64-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74e64-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74e64-131">Request body</span></span>
<span data-ttu-id="74e64-132">В тексте запроса укажите объект JSON, включающий параметр **POST** .</span><span class="sxs-lookup"><span data-stu-id="74e64-132">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="74e64-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="74e64-133">Parameter</span></span>    | <span data-ttu-id="74e64-134">Тип</span><span class="sxs-lookup"><span data-stu-id="74e64-134">Type</span></span>   |<span data-ttu-id="74e64-135">Описание</span><span class="sxs-lookup"><span data-stu-id="74e64-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74e64-136">post</span><span class="sxs-lookup"><span data-stu-id="74e64-136">post</span></span>|[<span data-ttu-id="74e64-137">post</span><span class="sxs-lookup"><span data-stu-id="74e64-137">post</span></span>](../resources/post.md)|<span data-ttu-id="74e64-138">Новая запись, с которой отправляются ответы, которые включают одно или несколько вложений [](../resources/attachment.md) в коллекцию вложений.</span><span class="sxs-lookup"><span data-stu-id="74e64-138">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="74e64-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e64-139">Response</span></span>

<span data-ttu-id="74e64-p104">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="74e64-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74e64-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="74e64-142">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="74e64-143">Пример 1: включение вложенного файла</span><span class="sxs-lookup"><span data-stu-id="74e64-143">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="74e64-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e64-144">Request</span></span>
<span data-ttu-id="74e64-145">Ниже приведен пример запроса, включающего файл в качестве вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="74e64-145">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74e64-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="74e64-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="74e64-147">C#</span><span class="sxs-lookup"><span data-stu-id="74e64-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74e64-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e64-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74e64-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74e64-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="74e64-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e64-150">Response</span></span>
<span data-ttu-id="74e64-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74e64-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="74e64-152">Пример 2: включение вложения элемента</span><span class="sxs-lookup"><span data-stu-id="74e64-152">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="74e64-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e64-153">Request</span></span>
<span data-ttu-id="74e64-154">Ниже приведен пример запроса, включающего событие в виде вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="74e64-154">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

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


#### <a name="response"></a><span data-ttu-id="74e64-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e64-155">Response</span></span>
<span data-ttu-id="74e64-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74e64-156">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="74e64-157">Пример 3: включение вложения ссылки</span><span class="sxs-lookup"><span data-stu-id="74e64-157">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="74e64-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e64-158">Request</span></span>
<span data-ttu-id="74e64-159">Ниже приведен пример запроса, включающего вложение ссылки при создании записи.</span><span class="sxs-lookup"><span data-stu-id="74e64-159">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="74e64-160">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="74e64-160">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74e64-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="74e64-161">HTTP</span></span>](#tab/http)
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

# <a name="ctabcsharp"></a>[<span data-ttu-id="74e64-162">C#</span><span class="sxs-lookup"><span data-stu-id="74e64-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74e64-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e64-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74e64-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74e64-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74e64-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e64-165">Response</span></span>
<span data-ttu-id="74e64-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74e64-166">Here is an example of the response.</span></span>
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
