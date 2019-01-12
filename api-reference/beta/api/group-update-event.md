---
title: Обновление события
description: Обновление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 092e5fdb8f70ec73d1c8a33230f596b9fdbf3b19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980001"
---
# <a name="update-event"></a><span data-ttu-id="dbbe3-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="dbbe3-103">Update event</span></span>

> <span data-ttu-id="dbbe3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbbe3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbbe3-106">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-106">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbbe3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbbe3-107">Permissions</span></span>
<span data-ttu-id="dbbe3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbbe3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbbe3-110">Permission type</span></span>      | <span data-ttu-id="dbbe3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbbe3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dbbe3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbbe3-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbbe3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbbe3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-115">Not supported.</span></span>    |
|<span data-ttu-id="dbbe3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbbe3-116">Application</span></span> | <span data-ttu-id="dbbe3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbbe3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbbe3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dbbe3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbbe3-119">Request headers</span></span>
| <span data-ttu-id="dbbe3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dbbe3-120">Name</span></span>       | <span data-ttu-id="dbbe3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dbbe3-121">Type</span></span> | <span data-ttu-id="dbbe3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dbbe3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbbe3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbbe3-123">Authorization</span></span>  | <span data-ttu-id="dbbe3-124">string</span><span class="sxs-lookup"><span data-stu-id="dbbe3-124">string</span></span>  | <span data-ttu-id="dbbe3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbbe3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbbe3-127">Request body</span></span>
<span data-ttu-id="dbbe3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="dbbe3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbbe3-131">Response</span></span>
<span data-ttu-id="dbbe3-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dbbe3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dbbe3-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dbbe3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbbe3-134">Request</span></span>
<span data-ttu-id="dbbe3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-135">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="dbbe3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbbe3-136">Response</span></span>
<span data-ttu-id="dbbe3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-137">The following is an example of the response.</span></span>

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
