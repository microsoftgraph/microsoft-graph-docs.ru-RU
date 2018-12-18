---
title: Обновление цепочки беседы
description: Обновление объекта thread.
author: dkershaw10
ms.openlocfilehash: db4b30d50bd616680f88949906cb96480668c612
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348596"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="2ec3e-103">Обновление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="2ec3e-103">Update conversation thread</span></span>
<span data-ttu-id="2ec3e-104">Обновление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="2ec3e-104">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec3e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ec3e-105">Permissions</span></span>
<span data-ttu-id="2ec3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ec3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ec3e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ec3e-108">Permission type</span></span>      | <span data-ttu-id="2ec3e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ec3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ec3e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ec3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ec3e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ec3e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ec3e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ec3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec3e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-113">Not supported.</span></span>    |
|<span data-ttu-id="2ec3e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ec3e-114">Application</span></span> | <span data-ttu-id="2ec3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ec3e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ec3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ec3e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ec3e-117">Request headers</span></span>
| <span data-ttu-id="2ec3e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2ec3e-118">Name</span></span>       | <span data-ttu-id="2ec3e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2ec3e-119">Type</span></span> | <span data-ttu-id="2ec3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ec3e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2ec3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ec3e-121">Authorization</span></span>  | <span data-ttu-id="2ec3e-122">string</span><span class="sxs-lookup"><span data-stu-id="2ec3e-122">string</span></span>  | <span data-ttu-id="2ec3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ec3e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ec3e-125">Request body</span></span>
<span data-ttu-id="2ec3e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="2ec3e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ec3e-129">Response</span></span>
<span data-ttu-id="2ec3e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ec3e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ec3e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2ec3e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ec3e-132">Request</span></span>
<span data-ttu-id="2ec3e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="2ec3e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ec3e-134">Response</span></span>
<span data-ttu-id="2ec3e-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ec3e-135">The following is an example of the response.</span></span>

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