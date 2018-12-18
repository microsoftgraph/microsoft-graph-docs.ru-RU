---
title: Добавление вложения
description: Используйте этот интерфейс API для добавления вложения в сообщение. Начиная с него
author: dkershaw10
ms.openlocfilehash: 67e219c7ffd95a41926be97323a2215625b30d2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328345"
---
# <a name="add-attachment"></a><span data-ttu-id="d323c-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="d323c-104">Add attachment</span></span>

> <span data-ttu-id="d323c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d323c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d323c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d323c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d323c-p103">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="d323c-p103">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="d323c-109">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="d323c-109">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="d323c-110">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d323c-110">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="d323c-111">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d323c-111">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="d323c-112">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="d323c-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="d323c-113">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="d323c-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d323c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d323c-114">Permissions</span></span>
<span data-ttu-id="d323c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d323c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d323c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d323c-117">Permission type</span></span>      | <span data-ttu-id="d323c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d323c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d323c-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d323c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d323c-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d323c-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d323c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d323c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d323c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d323c-122">Not supported.</span></span>    |
|<span data-ttu-id="d323c-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d323c-123">Application</span></span> | <span data-ttu-id="d323c-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d323c-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d323c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d323c-125">HTTP request</span></span>
<span data-ttu-id="d323c-126"><!-- { "blockType": "ignored" } -->Вложения для [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , относящегося к [беседе](../resources/conversation.md) группы.</span><span class="sxs-lookup"><span data-stu-id="d323c-126"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="d323c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d323c-127">Request headers</span></span>
| <span data-ttu-id="d323c-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d323c-128">Header</span></span>       | <span data-ttu-id="d323c-129">Значение</span><span class="sxs-lookup"><span data-stu-id="d323c-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d323c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d323c-130">Authorization</span></span>  | <span data-ttu-id="d323c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d323c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d323c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d323c-133">Request body</span></span>
<span data-ttu-id="d323c-134">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d323c-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d323c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d323c-135">Response</span></span>

<span data-ttu-id="d323c-136">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d323c-136">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="d323c-137">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="d323c-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d323c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d323c-138">Request</span></span>
<span data-ttu-id="d323c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d323c-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="d323c-140">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d323c-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d323c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d323c-141">Response</span></span>
<span data-ttu-id="d323c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d323c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="d323c-145">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="d323c-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d323c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d323c-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="d323c-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="d323c-147">Response</span></span>
<span data-ttu-id="d323c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d323c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a><span data-ttu-id="d323c-151">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="d323c-151">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d323c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d323c-152">Request</span></span>
<span data-ttu-id="d323c-153">Ниже приведен пример запроса, добавляет подключение к ссылку на сообщение.</span><span class="sxs-lookup"><span data-stu-id="d323c-153">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="d323c-154">Вложение указывает на папку на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d323c-154">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```

##### <a name="response"></a><span data-ttu-id="d323c-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="d323c-155">Response</span></span>
<span data-ttu-id="d323c-156">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="d323c-156">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
