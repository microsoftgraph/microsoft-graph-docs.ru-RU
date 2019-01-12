---
title: Обновление цепочки беседы
description: Обновление объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: defb7560a1d407a60ac813154ebd978f554e9763
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966260"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="e8520-103">Обновление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="e8520-103">Update conversation thread</span></span>

> <span data-ttu-id="e8520-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8520-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8520-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8520-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8520-106">Обновление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="e8520-106">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8520-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8520-107">Permissions</span></span>
<span data-ttu-id="e8520-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8520-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8520-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8520-110">Permission type</span></span>      | <span data-ttu-id="e8520-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8520-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8520-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8520-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8520-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8520-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8520-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8520-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8520-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8520-115">Not supported.</span></span>    |
|<span data-ttu-id="e8520-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8520-116">Application</span></span> | <span data-ttu-id="e8520-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8520-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8520-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8520-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8520-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8520-119">Request headers</span></span>
| <span data-ttu-id="e8520-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e8520-120">Name</span></span>       | <span data-ttu-id="e8520-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e8520-121">Type</span></span> | <span data-ttu-id="e8520-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e8520-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8520-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8520-123">Authorization</span></span>  | <span data-ttu-id="e8520-124">string</span><span class="sxs-lookup"><span data-stu-id="e8520-124">string</span></span>  | <span data-ttu-id="e8520-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8520-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8520-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8520-127">Request body</span></span>
<span data-ttu-id="e8520-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e8520-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="e8520-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8520-131">Response</span></span>
<span data-ttu-id="e8520-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8520-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8520-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e8520-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e8520-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8520-134">Request</span></span>
<span data-ttu-id="e8520-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8520-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="e8520-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8520-136">Response</span></span>
<span data-ttu-id="e8520-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8520-137">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
