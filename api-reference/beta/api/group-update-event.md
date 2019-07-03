---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2dba8ba7fb99fd8fa16fd65b9423eed15429b603
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442757"
---
# <a name="update-event"></a><span data-ttu-id="ef1e7-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="ef1e7-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef1e7-104">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="ef1e7-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1e7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef1e7-105">Permissions</span></span>
<span data-ttu-id="ef1e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef1e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef1e7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef1e7-108">Permission type</span></span>      | <span data-ttu-id="ef1e7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef1e7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef1e7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1e7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef1e7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1e7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-113">Not supported.</span></span>    |
|<span data-ttu-id="ef1e7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef1e7-114">Application</span></span> | <span data-ttu-id="ef1e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef1e7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef1e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ef1e7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef1e7-117">Request headers</span></span>
| <span data-ttu-id="ef1e7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ef1e7-118">Name</span></span>       | <span data-ttu-id="ef1e7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ef1e7-119">Type</span></span> | <span data-ttu-id="ef1e7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ef1e7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef1e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1e7-121">Authorization</span></span>  | <span data-ttu-id="ef1e7-122">string</span><span class="sxs-lookup"><span data-stu-id="ef1e7-122">string</span></span>  | <span data-ttu-id="ef1e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef1e7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef1e7-125">Request body</span></span>
<span data-ttu-id="ef1e7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ef1e7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef1e7-129">Response</span></span>
<span data-ttu-id="ef1e7-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef1e7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ef1e7-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ef1e7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef1e7-132">Request</span></span>
<span data-ttu-id="ef1e7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef1e7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1e7-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef1e7-135">C#</span><span class="sxs-lookup"><span data-stu-id="ef1e7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef1e7-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef1e7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef1e7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef1e7-137">Response</span></span>
<span data-ttu-id="ef1e7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-138">The following is an example of the response.</span></span>

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
