---
title: Создание вложения
description: Используйте этот API, чтобы добавить вложение в объект outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4f9386e680bb344055c62063232d5a8603fe42f
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994738"
---
# <a name="create-attachment"></a><span data-ttu-id="b86bd-103">Создание вложения</span><span class="sxs-lookup"><span data-stu-id="b86bd-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b86bd-104">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) в объект [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="b86bd-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="b86bd-105">Вложение может представлять собой файл (из типа [fileAttachment](../resources/fileattachment.md) ) или элемент Outlook (тип[itemAttachment](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="b86bd-105">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="b86bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b86bd-106">Permissions</span></span>

<span data-ttu-id="b86bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b86bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b86bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b86bd-109">Permission type</span></span>      | <span data-ttu-id="b86bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b86bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b86bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b86bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b86bd-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b86bd-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b86bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b86bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b86bd-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b86bd-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b86bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b86bd-115">Application</span></span> | <span data-ttu-id="b86bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b86bd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b86bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b86bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="b86bd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b86bd-118">Request headers</span></span>

| <span data-ttu-id="b86bd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b86bd-119">Name</span></span>       | <span data-ttu-id="b86bd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b86bd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b86bd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b86bd-121">Authorization</span></span>  | <span data-ttu-id="b86bd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b86bd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b86bd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b86bd-124">Content-Type</span></span> | <span data-ttu-id="b86bd-125">Строка, представляющая тип данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="b86bd-125">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="b86bd-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b86bd-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b86bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b86bd-127">Request body</span></span>

<span data-ttu-id="b86bd-128">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b86bd-128">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b86bd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b86bd-129">Response</span></span>

<span data-ttu-id="b86bd-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b86bd-130">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b86bd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b86bd-131">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="b86bd-132">Пример 1: Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="b86bd-132">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="b86bd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b86bd-133">Request</span></span>

<span data-ttu-id="b86bd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b86bd-134">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="b86bd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b86bd-135">Response</span></span>

<span data-ttu-id="b86bd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b86bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="b86bd-139">Пример 2: Добавление вложения элемента</span><span class="sxs-lookup"><span data-stu-id="b86bd-139">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="b86bd-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b86bd-140">Request</span></span>

<span data-ttu-id="b86bd-141">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="b86bd-141">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


#### <a name="response"></a><span data-ttu-id="b86bd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b86bd-142">Response</span></span>

<span data-ttu-id="b86bd-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b86bd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
