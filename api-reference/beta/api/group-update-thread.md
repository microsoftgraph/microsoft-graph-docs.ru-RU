---
title: Обновление цепочки беседы
description: Обновление объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 90dc41de34a807b72f05203c08197fcb4bc5eb97
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510619"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="98eab-103">Обновление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="98eab-103">Update conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98eab-104">Обновление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="98eab-104">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98eab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98eab-105">Permissions</span></span>
<span data-ttu-id="98eab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98eab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98eab-108">Permission type</span></span>      | <span data-ttu-id="98eab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98eab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98eab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98eab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98eab-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98eab-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98eab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98eab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98eab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98eab-113">Not supported.</span></span>    |
|<span data-ttu-id="98eab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98eab-114">Application</span></span> | <span data-ttu-id="98eab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98eab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98eab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98eab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="98eab-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98eab-117">Request headers</span></span>
| <span data-ttu-id="98eab-118">Имя</span><span class="sxs-lookup"><span data-stu-id="98eab-118">Name</span></span>       | <span data-ttu-id="98eab-119">Тип</span><span class="sxs-lookup"><span data-stu-id="98eab-119">Type</span></span> | <span data-ttu-id="98eab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="98eab-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98eab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98eab-121">Authorization</span></span>  | <span data-ttu-id="98eab-122">string</span><span class="sxs-lookup"><span data-stu-id="98eab-122">string</span></span>  | <span data-ttu-id="98eab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98eab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98eab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98eab-125">Request body</span></span>
<span data-ttu-id="98eab-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="98eab-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="98eab-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="98eab-129">Response</span></span>
<span data-ttu-id="98eab-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98eab-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98eab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98eab-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="98eab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98eab-132">Request</span></span>
<span data-ttu-id="98eab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98eab-133">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="98eab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98eab-134">Response</span></span>
<span data-ttu-id="98eab-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98eab-135">The following is an example of the response.</span></span>

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
    "Error: /api-reference/beta/api/group-update-thread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
