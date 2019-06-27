---
title: Удаление события
description: Удаление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 77e81d0d14c12b11612ab5917d1858256fa1ab28
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275819"
---
# <a name="delete-event"></a><span data-ttu-id="300f2-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="300f2-103">Delete event</span></span>
<span data-ttu-id="300f2-104">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="300f2-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="300f2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="300f2-105">Permissions</span></span>
<span data-ttu-id="300f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="300f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="300f2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="300f2-108">Permission type</span></span>      | <span data-ttu-id="300f2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="300f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="300f2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="300f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="300f2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="300f2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="300f2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="300f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="300f2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300f2-113">Not supported.</span></span>    |
|<span data-ttu-id="300f2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="300f2-114">Application</span></span> | <span data-ttu-id="300f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300f2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="300f2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="300f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="300f2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="300f2-117">Request headers</span></span>
| <span data-ttu-id="300f2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="300f2-118">Name</span></span>       | <span data-ttu-id="300f2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="300f2-119">Type</span></span> | <span data-ttu-id="300f2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="300f2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="300f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="300f2-121">Authorization</span></span>  | <span data-ttu-id="300f2-122">string</span><span class="sxs-lookup"><span data-stu-id="300f2-122">string</span></span>  | <span data-ttu-id="300f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="300f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="300f2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="300f2-125">Request body</span></span>
<span data-ttu-id="300f2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="300f2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="300f2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="300f2-127">Response</span></span>
<span data-ttu-id="300f2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="300f2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="300f2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="300f2-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="300f2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="300f2-131">Request</span></span>
<span data-ttu-id="300f2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="300f2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="300f2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="300f2-133">Response</span></span>
<span data-ttu-id="300f2-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="300f2-134">The following is an example of the response.</span></span> 
><span data-ttu-id="300f2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="300f2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="300f2-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="300f2-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="300f2-138">C#</span><span class="sxs-lookup"><span data-stu-id="300f2-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="300f2-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="300f2-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="300f2-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="300f2-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_group_event-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-event.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-delete-event.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-event.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
