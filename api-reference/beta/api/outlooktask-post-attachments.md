---
title: Создание вложения
description: Используйте этот API, чтобы добавить вложение в объект outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d81c0c9b3c59e41c1df42f2af446a61d7bb1a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456182"
---
# <a name="create-attachment"></a><span data-ttu-id="7d0be-103">Создание вложения</span><span class="sxs-lookup"><span data-stu-id="7d0be-103">Create attachment</span></span>

<span data-ttu-id="7d0be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d0be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d0be-105">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) в объект [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="7d0be-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="7d0be-106">Вложение может представлять собой файл (из типа [fileAttachment](../resources/fileattachment.md) ) или элемент Outlook (тип[itemAttachment](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="7d0be-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d0be-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0be-107">Permissions</span></span>

<span data-ttu-id="7d0be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d0be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d0be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0be-110">Permission type</span></span>      | <span data-ttu-id="7d0be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d0be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d0be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d0be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d0be-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0be-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7d0be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d0be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d0be-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0be-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7d0be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d0be-116">Application</span></span> | <span data-ttu-id="7d0be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d0be-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d0be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d0be-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="7d0be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d0be-119">Request headers</span></span>

| <span data-ttu-id="7d0be-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7d0be-120">Name</span></span>       | <span data-ttu-id="7d0be-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7d0be-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d0be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d0be-122">Authorization</span></span>  | <span data-ttu-id="7d0be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d0be-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d0be-125">Content-Type</span></span> | <span data-ttu-id="7d0be-126">Строка, представляющая тип данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="7d0be-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="7d0be-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="7d0be-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d0be-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d0be-128">Request body</span></span>

<span data-ttu-id="7d0be-129">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d0be-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7d0be-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0be-130">Response</span></span>

<span data-ttu-id="7d0be-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d0be-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d0be-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d0be-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="7d0be-133">Пример 1: Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="7d0be-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="7d0be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d0be-134">Request</span></span>

<span data-ttu-id="7d0be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d0be-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d0be-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d0be-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7d0be-137">C#</span><span class="sxs-lookup"><span data-stu-id="7d0be-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d0be-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d0be-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d0be-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d0be-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d0be-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0be-140">Response</span></span>

<span data-ttu-id="7d0be-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="7d0be-144">Пример 2: Добавление вложения элемента</span><span class="sxs-lookup"><span data-stu-id="7d0be-144">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="7d0be-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d0be-145">Request</span></span>

<span data-ttu-id="7d0be-146">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="7d0be-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


#### <a name="response"></a><span data-ttu-id="7d0be-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0be-147">Response</span></span>

<span data-ttu-id="7d0be-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
