---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4694f7e9435f886538f7d4d6e21b141e3fd470b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323124"
---
# <a name="update-event"></a><span data-ttu-id="b69bf-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="b69bf-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b69bf-104">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b69bf-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b69bf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b69bf-105">Permissions</span></span>
<span data-ttu-id="b69bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b69bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b69bf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b69bf-108">Permission type</span></span>      | <span data-ttu-id="b69bf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b69bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b69bf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b69bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b69bf-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b69bf-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b69bf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b69bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b69bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b69bf-113">Not supported.</span></span>    |
|<span data-ttu-id="b69bf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b69bf-114">Application</span></span> | <span data-ttu-id="b69bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b69bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b69bf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b69bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b69bf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b69bf-117">Request headers</span></span>
| <span data-ttu-id="b69bf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b69bf-118">Name</span></span>       | <span data-ttu-id="b69bf-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b69bf-119">Type</span></span> | <span data-ttu-id="b69bf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b69bf-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b69bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b69bf-121">Authorization</span></span>  | <span data-ttu-id="b69bf-122">string</span><span class="sxs-lookup"><span data-stu-id="b69bf-122">string</span></span>  | <span data-ttu-id="b69bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b69bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b69bf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b69bf-125">Request body</span></span>
<span data-ttu-id="b69bf-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b69bf-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b69bf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b69bf-129">Response</span></span>
<span data-ttu-id="b69bf-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b69bf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b69bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b69bf-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b69bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b69bf-132">Request</span></span>
<span data-ttu-id="b69bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b69bf-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b69bf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b69bf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b69bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="b69bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b69bf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b69bf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b69bf-137">Java</span><span class="sxs-lookup"><span data-stu-id="b69bf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b69bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b69bf-138">Response</span></span>
<span data-ttu-id="b69bf-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b69bf-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
