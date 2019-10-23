---
title: Добавление вложения
description: Добавление вложения при создании записи группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b8e6a59dc0d8bf20ddac6c39c4c92081061d2946
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632693"
---
# <a name="add-attachment"></a><span data-ttu-id="4600f-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="4600f-103">Add attachment</span></span>

<span data-ttu-id="4600f-104">Добавление [вложения](../resources/attachment.md) при создании записи группы.</span><span class="sxs-lookup"><span data-stu-id="4600f-104">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span>

<span data-ttu-id="4600f-105">Эта операция ограничит размер вложения, которое можно добавить в течение 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="4600f-105">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="4600f-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="4600f-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4600f-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4600f-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4600f-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4600f-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="4600f-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4600f-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4600f-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4600f-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4600f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4600f-111">Permissions</span></span>
<span data-ttu-id="4600f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4600f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4600f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4600f-114">Permission type</span></span>      | <span data-ttu-id="4600f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4600f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4600f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4600f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4600f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4600f-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4600f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4600f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4600f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4600f-119">Not supported.</span></span>    |
|<span data-ttu-id="4600f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4600f-120">Application</span></span> | <span data-ttu-id="4600f-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4600f-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4600f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4600f-122">HTTP request</span></span>
<span data-ttu-id="4600f-123">Включите вложение при создании [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="4600f-123">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="4600f-124">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="4600f-124">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="4600f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4600f-125">Request headers</span></span>
| <span data-ttu-id="4600f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4600f-126">Header</span></span>       | <span data-ttu-id="4600f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="4600f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4600f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4600f-128">Authorization</span></span>  | <span data-ttu-id="4600f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4600f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4600f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4600f-131">Request body</span></span>
<span data-ttu-id="4600f-132">В тексте запроса укажите объект JSON, включающий параметр **POST** .</span><span class="sxs-lookup"><span data-stu-id="4600f-132">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="4600f-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="4600f-133">Parameter</span></span>    | <span data-ttu-id="4600f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4600f-134">Type</span></span>   |<span data-ttu-id="4600f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4600f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4600f-136">post</span><span class="sxs-lookup"><span data-stu-id="4600f-136">post</span></span>|[<span data-ttu-id="4600f-137">post</span><span class="sxs-lookup"><span data-stu-id="4600f-137">post</span></span>](../resources/post.md)|<span data-ttu-id="4600f-138">Новая запись, с которой отправляются ответы, которые включают одно или несколько вложений в коллекцию [вложений](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="4600f-138">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="4600f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4600f-139">Response</span></span>

<span data-ttu-id="4600f-p104">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="4600f-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4600f-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="4600f-142">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="4600f-143">Пример 1: включение вложенного файла</span><span class="sxs-lookup"><span data-stu-id="4600f-143">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="4600f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4600f-144">Request</span></span>
<span data-ttu-id="4600f-145">Ниже приведен пример запроса, включающего файл в качестве вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="4600f-145">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4600f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4600f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4600f-147">C#</span><span class="sxs-lookup"><span data-stu-id="4600f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4600f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4600f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4600f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4600f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4600f-150">Java</span><span class="sxs-lookup"><span data-stu-id="4600f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4600f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4600f-151">Response</span></span>
<span data-ttu-id="4600f-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4600f-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="4600f-153">Пример 2: включение вложения элемента</span><span class="sxs-lookup"><span data-stu-id="4600f-153">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4600f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4600f-154">Request</span></span>
<span data-ttu-id="4600f-155">Ниже приведен пример запроса, включающего событие в виде вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="4600f-155">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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


#### <a name="response"></a><span data-ttu-id="4600f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4600f-156">Response</span></span>
<span data-ttu-id="4600f-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4600f-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="4600f-158">Пример 3: включение вложения ссылки</span><span class="sxs-lookup"><span data-stu-id="4600f-158">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4600f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4600f-159">Request</span></span>
<span data-ttu-id="4600f-160">Ниже приведен пример запроса, включающего вложение ссылки при создании записи.</span><span class="sxs-lookup"><span data-stu-id="4600f-160">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="4600f-161">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4600f-161">The attachment points to a folder on OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4600f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4600f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4600f-163">C#</span><span class="sxs-lookup"><span data-stu-id="4600f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4600f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4600f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4600f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4600f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4600f-166">Java</span><span class="sxs-lookup"><span data-stu-id="4600f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4600f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4600f-167">Response</span></span>
<span data-ttu-id="4600f-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4600f-168">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
