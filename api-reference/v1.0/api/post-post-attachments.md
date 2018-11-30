---
title: Добавление вложения
description: Используйте этот интерфейс API для добавления вложения в сообщение. Начиная с него
ms.openlocfilehash: bf3e58fe8d6131184cac87d3ab4433ba41a18034
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028009"
---
# <a name="add-attachment"></a><span data-ttu-id="f1f85-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="f1f85-104">Add attachment</span></span>

<span data-ttu-id="f1f85-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="f1f85-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="f1f85-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="f1f85-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f1f85-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="f1f85-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f1f85-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="f1f85-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f1f85-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f1f85-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f1f85-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f1f85-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f1f85-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1f85-112">Permissions</span></span>
<span data-ttu-id="f1f85-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f85-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f85-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1f85-115">Permission type</span></span>      | <span data-ttu-id="f1f85-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1f85-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1f85-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1f85-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f1f85-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f85-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1f85-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1f85-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1f85-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1f85-120">Not supported.</span></span>    |
|<span data-ttu-id="f1f85-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1f85-121">Application</span></span> | <span data-ttu-id="f1f85-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f85-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1f85-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1f85-123">HTTP request</span></span>
<span data-ttu-id="f1f85-124"><!-- { "blockType": "ignored" } -->Вложения для [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , относящегося к [беседе](../resources/conversation.md) группы.</span><span class="sxs-lookup"><span data-stu-id="f1f85-124"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f1f85-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1f85-125">Request headers</span></span>
| <span data-ttu-id="f1f85-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1f85-126">Header</span></span>       | <span data-ttu-id="f1f85-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f1f85-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1f85-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1f85-128">Authorization</span></span>  | <span data-ttu-id="f1f85-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1f85-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1f85-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1f85-131">Request body</span></span>
<span data-ttu-id="f1f85-132">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1f85-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f1f85-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1f85-133">Response</span></span>

<span data-ttu-id="f1f85-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1f85-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f1f85-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="f1f85-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f1f85-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1f85-136">Request</span></span>
<span data-ttu-id="f1f85-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1f85-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="f1f85-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1f85-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f1f85-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1f85-139">Response</span></span>
<span data-ttu-id="f1f85-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f1f85-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="f1f85-143">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="f1f85-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f1f85-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1f85-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="f1f85-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1f85-145">Response</span></span>
<span data-ttu-id="f1f85-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f1f85-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
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
