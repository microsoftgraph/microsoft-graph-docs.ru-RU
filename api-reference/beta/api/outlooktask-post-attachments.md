---
title: Создание вложения
description: Используйте этот API, чтобы добавить вложение в объект outlookTask.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5cc6bf02fceef6467f7d32232c873517c797bd3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413619"
---
# <a name="create-attachment"></a><span data-ttu-id="4e4d9-103">Создание вложения</span><span class="sxs-lookup"><span data-stu-id="4e4d9-103">Create attachment</span></span>

<span data-ttu-id="4e4d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e4d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e4d9-105">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) в объект [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="4e4d9-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="4e4d9-106">Вложение может представлять собой файл (из типа [fileAttachment](../resources/fileattachment.md) ) или элемент Outlook (тип[itemAttachment](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="4e4d9-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e4d9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4d9-107">Permissions</span></span>

<span data-ttu-id="4e4d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e4d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e4d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4d9-110">Permission type</span></span>      | <span data-ttu-id="4e4d9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e4d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e4d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e4d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e4d9-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e4d9-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4e4d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e4d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e4d9-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e4d9-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4e4d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e4d9-116">Application</span></span> | <span data-ttu-id="4e4d9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e4d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e4d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="4e4d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e4d9-119">Request headers</span></span>

| <span data-ttu-id="4e4d9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4e4d9-120">Name</span></span>       | <span data-ttu-id="4e4d9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e4d9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e4d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e4d9-122">Authorization</span></span>  | <span data-ttu-id="4e4d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e4d9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e4d9-125">Content-Type</span></span> | <span data-ttu-id="4e4d9-126">Строка, представляющая тип данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="4e4d9-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e4d9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e4d9-128">Request body</span></span>

<span data-ttu-id="4e4d9-129">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4e4d9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4d9-130">Response</span></span>

<span data-ttu-id="4e4d9-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e4d9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="4e4d9-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="4e4d9-133">Пример 1: Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="4e4d9-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="4e4d9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e4d9-134">Request</span></span>

<span data-ttu-id="4e4d9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e4d9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e4d9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_file_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```
# <a name="c"></a>[<span data-ttu-id="4e4d9-137">C#</span><span class="sxs-lookup"><span data-stu-id="4e4d9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e4d9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e4d9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e4d9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e4d9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e4d9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4d9-140">Response</span></span>

<span data-ttu-id="4e4d9-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_file_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP 201 Created

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "text/plain",
    "id": "AAMkADAAAANXbdnAAABEgAQAKQF4_X0QwVHpmAmxUgHN_Q=",
    "lastModifiedDateTime": "2020-01-07T22:13:30Z",
    "name": "menu.txt",
    "contentType": "text/plain",
    "size": 178,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="4e4d9-144">Пример 2: Добавление вложения элемента</span><span class="sxs-lookup"><span data-stu-id="4e4d9-144">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4e4d9-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e4d9-145">Request</span></span>

<span data-ttu-id="4e4d9-146">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_item_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

{
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
             "dateTime": "2020-01-12T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2020-01-12T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```


#### <a name="response"></a><span data-ttu-id="4e4d9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4d9-147">Response</span></span>

<span data-ttu-id="4e4d9-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e4d9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_item_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADAAAANXbdnAAABEgAQANgBvaZHiKVMskpdj1k9KEQ=",
    "lastModifiedDateTime": "2020-01-07T22:18:11Z",
    "name": "Holiday event",
    "contentType": null,
    "size": 2067,
    "isInline": false
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
