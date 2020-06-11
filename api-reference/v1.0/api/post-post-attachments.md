---
title: Добавление вложения
description: Добавление вложения при создании записи группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 79d0035a0ee14fa047bd02b77e3a35cfa9b82ada
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682076"
---
# <a name="add-attachment"></a><span data-ttu-id="8d065-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="8d065-103">Add attachment</span></span>

<span data-ttu-id="8d065-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d065-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d065-105">Добавление [вложения](../resources/attachment.md) при создании записи группы.</span><span class="sxs-lookup"><span data-stu-id="8d065-105">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span>

<span data-ttu-id="8d065-106">Эта операция ограничит размер вложения, которое можно добавить в течение 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="8d065-106">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="8d065-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="8d065-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="8d065-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="8d065-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="8d065-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="8d065-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="8d065-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="8d065-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="8d065-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="8d065-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d065-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d065-112">Permissions</span></span>
<span data-ttu-id="8d065-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d065-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d065-115">Permission type</span></span>      | <span data-ttu-id="8d065-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d065-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d065-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d065-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8d065-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d065-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d065-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d065-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d065-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d065-120">Not supported.</span></span>    |
|<span data-ttu-id="8d065-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d065-121">Application</span></span> | <span data-ttu-id="8d065-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d065-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d065-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d065-123">HTTP request</span></span>
<span data-ttu-id="8d065-124">Включите вложение при создании [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="8d065-124">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="8d065-125">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="8d065-125">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="8d065-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d065-126">Request headers</span></span>
| <span data-ttu-id="8d065-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d065-127">Header</span></span>       | <span data-ttu-id="8d065-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8d065-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d065-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d065-129">Authorization</span></span>  | <span data-ttu-id="8d065-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d065-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d065-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d065-132">Request body</span></span>
<span data-ttu-id="8d065-133">В тексте запроса укажите объект JSON, включающий параметр **POST** .</span><span class="sxs-lookup"><span data-stu-id="8d065-133">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="8d065-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="8d065-134">Parameter</span></span>    | <span data-ttu-id="8d065-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8d065-135">Type</span></span>   |<span data-ttu-id="8d065-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8d065-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d065-137">post</span><span class="sxs-lookup"><span data-stu-id="8d065-137">post</span></span>|[<span data-ttu-id="8d065-138">post</span><span class="sxs-lookup"><span data-stu-id="8d065-138">post</span></span>](../resources/post.md)|<span data-ttu-id="8d065-139">Новая запись, с которой отправляются ответы, которые включают одно или несколько вложений в коллекцию [вложений](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="8d065-139">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="8d065-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d065-140">Response</span></span>

<span data-ttu-id="8d065-p104">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="8d065-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d065-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d065-143">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="8d065-144">Пример 1: включение вложенного файла</span><span class="sxs-lookup"><span data-stu-id="8d065-144">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="8d065-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d065-145">Request</span></span>
<span data-ttu-id="8d065-146">Ниже приведен пример запроса, включающего файл в качестве вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="8d065-146">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d065-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d065-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d065-148">C#</span><span class="sxs-lookup"><span data-stu-id="8d065-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d065-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d065-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d065-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d065-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d065-151">Java</span><span class="sxs-lookup"><span data-stu-id="8d065-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8d065-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d065-152">Response</span></span>
<span data-ttu-id="8d065-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d065-153">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="8d065-154">Пример 2: включение вложения элемента</span><span class="sxs-lookup"><span data-stu-id="8d065-154">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="8d065-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d065-155">Request</span></span>
<span data-ttu-id="8d065-156">Ниже приведен пример запроса, включающего событие в виде вложения при создании записи.</span><span class="sxs-lookup"><span data-stu-id="8d065-156">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

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


#### <a name="response"></a><span data-ttu-id="8d065-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d065-157">Response</span></span>
<span data-ttu-id="8d065-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d065-158">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="8d065-159">Пример 3: включение вложения ссылки</span><span class="sxs-lookup"><span data-stu-id="8d065-159">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="8d065-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d065-160">Request</span></span>
<span data-ttu-id="8d065-161">Ниже приведен пример запроса, включающего вложение ссылки при создании записи.</span><span class="sxs-lookup"><span data-stu-id="8d065-161">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="8d065-162">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8d065-162">The attachment points to a folder on OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d065-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d065-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d065-164">C#</span><span class="sxs-lookup"><span data-stu-id="8d065-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d065-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d065-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d065-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d065-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d065-167">Java</span><span class="sxs-lookup"><span data-stu-id="8d065-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d065-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d065-168">Response</span></span>
<span data-ttu-id="8d065-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d065-169">Here is an example of the response.</span></span>
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
