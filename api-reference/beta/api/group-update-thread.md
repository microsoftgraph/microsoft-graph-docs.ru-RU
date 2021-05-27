---
title: Обновление цепочки беседы
description: Обновление объекта thread.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 26eab98dc2d734e76905c458c7730d6f6237bc93
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681230"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="a5f4e-103">Обновление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="a5f4e-103">Update conversation thread</span></span>

<span data-ttu-id="a5f4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f4e-105">Обновление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="a5f4e-105">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5f4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f4e-106">Permissions</span></span>
<span data-ttu-id="a5f4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f4e-109">Permission type</span></span>      | <span data-ttu-id="a5f4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5f4e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5f4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5f4e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5f4e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f4e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5f4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5f4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5f4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-114">Not supported.</span></span>    |
|<span data-ttu-id="a5f4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5f4e-115">Application</span></span> | <span data-ttu-id="a5f4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5f4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5f4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5f4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5f4e-118">Request headers</span></span>
| <span data-ttu-id="a5f4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a5f4e-119">Name</span></span>       | <span data-ttu-id="a5f4e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a5f4e-120">Type</span></span> | <span data-ttu-id="a5f4e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f4e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5f4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f4e-122">Authorization</span></span>  | <span data-ttu-id="a5f4e-123">string</span><span class="sxs-lookup"><span data-stu-id="a5f4e-123">string</span></span>  | <span data-ttu-id="a5f4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5f4e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5f4e-126">Request body</span></span>
<span data-ttu-id="a5f4e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a5f4e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f4e-130">Response</span></span>
<span data-ttu-id="a5f4e-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5f4e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a5f4e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a5f4e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5f4e-133">Request</span></span>
<span data-ttu-id="a5f4e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5f4e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f4e-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="a5f4e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5f4e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5f4e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f4e-137">Response</span></span>
<span data-ttu-id="a5f4e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5f4e-138">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


