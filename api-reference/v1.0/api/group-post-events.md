---
title: Создание события
description: Этот API используется для создания события.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: f2cfa417ba5064fd91744d8ded48a7fb3621b67b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613750"
---
# <a name="create-event"></a><span data-ttu-id="f7ca8-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="f7ca8-103">Create event</span></span>
<span data-ttu-id="f7ca8-104">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="f7ca8-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7ca8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ca8-105">Permissions</span></span>
<span data-ttu-id="f7ca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ca8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ca8-108">Permission type</span></span>      | <span data-ttu-id="f7ca8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7ca8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7ca8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7ca8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7ca8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ca8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7ca8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7ca8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ca8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-113">Not supported.</span></span>    |
|<span data-ttu-id="f7ca8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7ca8-114">Application</span></span> | <span data-ttu-id="f7ca8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ca8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7ca8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="f7ca8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7ca8-117">Request headers</span></span>
| <span data-ttu-id="f7ca8-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7ca8-118">Header</span></span>       | <span data-ttu-id="f7ca8-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f7ca8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7ca8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7ca8-120">Authorization</span></span>  | <span data-ttu-id="f7ca8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7ca8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7ca8-123">Request body</span></span>
<span data-ttu-id="f7ca8-124">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f7ca8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ca8-125">Response</span></span>
<span data-ttu-id="f7ca8-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ca8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f7ca8-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7ca8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7ca8-128">Request</span></span>
<span data-ttu-id="f7ca8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

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
<span data-ttu-id="f7ca8-130">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="f7ca8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ca8-131">Response</span></span>
<span data-ttu-id="f7ca8-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-132">The following is an example of the response.</span></span>
><span data-ttu-id="f7ca8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7ca8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 285

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7ca8-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f7ca8-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7ca8-136">C#</span><span class="sxs-lookup"><span data-stu-id="f7ca8-136">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7ca8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7ca8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
