---
title: Создание вложения
description: Используйте этот API, чтобы добавить вложение в outlookTask.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 70e14b9e13656e61a17bb0d3dc7b393dcf36f9b4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474778"
---
# <a name="create-attachment-deprecated"></a><span data-ttu-id="b815a-103">Создание вложений (неподготовленных)</span><span class="sxs-lookup"><span data-stu-id="b815a-103">Create attachment (deprecated)</span></span>

<span data-ttu-id="b815a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b815a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="b815a-105">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) в [outlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="b815a-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="b815a-106">Вложение может быть файлом (типа [fileAttachment)](../resources/fileattachment.md) или элементом Outlook[(тип itemAttachment).](../resources/itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="b815a-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="b815a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b815a-107">Permissions</span></span>

<span data-ttu-id="b815a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b815a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b815a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b815a-110">Permission type</span></span>      | <span data-ttu-id="b815a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b815a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b815a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b815a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b815a-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b815a-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b815a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b815a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b815a-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b815a-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b815a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b815a-116">Application</span></span> | <span data-ttu-id="b815a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b815a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b815a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b815a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="b815a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b815a-119">Request headers</span></span>

| <span data-ttu-id="b815a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b815a-120">Name</span></span>       | <span data-ttu-id="b815a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b815a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b815a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b815a-122">Authorization</span></span>  | <span data-ttu-id="b815a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b815a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b815a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b815a-125">Content-Type</span></span> | <span data-ttu-id="b815a-126">Строка, которая представляет тип данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="b815a-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="b815a-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b815a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b815a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b815a-128">Request body</span></span>

<span data-ttu-id="b815a-129">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b815a-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b815a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b815a-130">Response</span></span>

<span data-ttu-id="b815a-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b815a-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b815a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b815a-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="b815a-133">Пример 1. Добавление вложения в файл</span><span class="sxs-lookup"><span data-stu-id="b815a-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="b815a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b815a-134">Request</span></span>

<span data-ttu-id="b815a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b815a-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b815a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b815a-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b815a-137">C#</span><span class="sxs-lookup"><span data-stu-id="b815a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b815a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b815a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b815a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b815a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b815a-140">Java</span><span class="sxs-lookup"><span data-stu-id="b815a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-file-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b815a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b815a-141">Response</span></span>

<span data-ttu-id="b815a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b815a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="b815a-145">Пример 2. Добавление вложения элемента</span><span class="sxs-lookup"><span data-stu-id="b815a-145">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="b815a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b815a-146">Request</span></span>

<span data-ttu-id="b815a-147">Вот пример, который прикрепит событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="b815a-147">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="b815a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b815a-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b815a-149">C#</span><span class="sxs-lookup"><span data-stu-id="b815a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-item-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b815a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b815a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-item-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b815a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b815a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-item-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b815a-152">Java</span><span class="sxs-lookup"><span data-stu-id="b815a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-item-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="b815a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b815a-153">Response</span></span>

<span data-ttu-id="b815a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b815a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


