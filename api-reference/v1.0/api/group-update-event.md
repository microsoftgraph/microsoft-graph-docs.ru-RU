---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9b6c61ba2e63fab0572a9efc76dccc56c581be0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613057"
---
# <a name="update-event"></a><span data-ttu-id="1343d-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="1343d-103">Update event</span></span>
<span data-ttu-id="1343d-104">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1343d-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1343d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1343d-105">Permissions</span></span>
<span data-ttu-id="1343d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1343d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1343d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1343d-108">Permission type</span></span>      | <span data-ttu-id="1343d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1343d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1343d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1343d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1343d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1343d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1343d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1343d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1343d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1343d-113">Not supported.</span></span>    |
|<span data-ttu-id="1343d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1343d-114">Application</span></span> | <span data-ttu-id="1343d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1343d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1343d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1343d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1343d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1343d-117">Request headers</span></span>
| <span data-ttu-id="1343d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1343d-118">Name</span></span>       | <span data-ttu-id="1343d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1343d-119">Type</span></span> | <span data-ttu-id="1343d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1343d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1343d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1343d-121">Authorization</span></span>  | <span data-ttu-id="1343d-122">string</span><span class="sxs-lookup"><span data-stu-id="1343d-122">string</span></span>  | <span data-ttu-id="1343d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1343d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1343d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1343d-125">Request body</span></span>
<span data-ttu-id="1343d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1343d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="1343d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1343d-129">Response</span></span>
<span data-ttu-id="1343d-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1343d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1343d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1343d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1343d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1343d-132">Request</span></span>
<span data-ttu-id="1343d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1343d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="1343d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1343d-134">Response</span></span>
<span data-ttu-id="1343d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1343d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1343d-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1343d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1343d-137">Языках</span><span class="sxs-lookup"><span data-stu-id="1343d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1343d-138">Язык</span><span class="sxs-lookup"><span data-stu-id="1343d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
