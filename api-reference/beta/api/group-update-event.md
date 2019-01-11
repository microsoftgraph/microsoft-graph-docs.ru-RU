---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1499ab66d698f8f22bde79d0ef3e53fdd8722302
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879228"
---
# <a name="update-event"></a><span data-ttu-id="45338-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="45338-103">Update event</span></span>

> <span data-ttu-id="45338-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45338-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45338-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45338-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45338-106">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="45338-106">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45338-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45338-107">Permissions</span></span>
<span data-ttu-id="45338-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45338-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45338-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45338-110">Permission type</span></span>      | <span data-ttu-id="45338-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45338-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45338-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45338-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45338-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45338-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45338-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45338-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45338-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45338-115">Not supported.</span></span>    |
|<span data-ttu-id="45338-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45338-116">Application</span></span> | <span data-ttu-id="45338-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45338-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45338-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45338-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45338-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45338-119">Request headers</span></span>
| <span data-ttu-id="45338-120">Имя</span><span class="sxs-lookup"><span data-stu-id="45338-120">Name</span></span>       | <span data-ttu-id="45338-121">Тип</span><span class="sxs-lookup"><span data-stu-id="45338-121">Type</span></span> | <span data-ttu-id="45338-122">Описание</span><span class="sxs-lookup"><span data-stu-id="45338-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45338-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45338-123">Authorization</span></span>  | <span data-ttu-id="45338-124">string</span><span class="sxs-lookup"><span data-stu-id="45338-124">string</span></span>  | <span data-ttu-id="45338-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45338-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45338-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45338-127">Request body</span></span>
<span data-ttu-id="45338-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="45338-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="45338-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="45338-131">Response</span></span>
<span data-ttu-id="45338-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45338-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45338-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45338-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45338-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45338-134">Request</span></span>
<span data-ttu-id="45338-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45338-135">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="45338-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45338-136">Response</span></span>
<span data-ttu-id="45338-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="45338-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
