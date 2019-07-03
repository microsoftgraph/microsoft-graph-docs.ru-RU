---
title: Удаление события
description: Удаление объекта event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3b1478076c9d176794d285d9997bc21b8271b658
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440703"
---
# <a name="delete-event"></a><span data-ttu-id="d8002-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="d8002-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8002-104">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d8002-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8002-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8002-105">Permissions</span></span>
<span data-ttu-id="d8002-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8002-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8002-108">Permission type</span></span>      | <span data-ttu-id="d8002-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8002-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8002-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8002-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8002-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8002-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8002-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8002-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8002-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8002-113">Not supported.</span></span>    |
|<span data-ttu-id="d8002-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8002-114">Application</span></span> | <span data-ttu-id="d8002-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8002-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8002-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8002-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8002-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8002-117">Request headers</span></span>
| <span data-ttu-id="d8002-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d8002-118">Name</span></span>       | <span data-ttu-id="d8002-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d8002-119">Type</span></span> | <span data-ttu-id="d8002-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d8002-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8002-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8002-121">Authorization</span></span>  | <span data-ttu-id="d8002-122">string</span><span class="sxs-lookup"><span data-stu-id="d8002-122">string</span></span>  | <span data-ttu-id="d8002-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8002-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8002-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8002-125">Request body</span></span>
<span data-ttu-id="d8002-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8002-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8002-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8002-127">Response</span></span>
<span data-ttu-id="d8002-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d8002-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8002-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8002-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d8002-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8002-131">Request</span></span>
<span data-ttu-id="d8002-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8002-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8002-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8002-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8002-134">C#</span><span class="sxs-lookup"><span data-stu-id="d8002-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8002-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8002-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8002-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d8002-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d8002-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8002-137">Response</span></span>
<span data-ttu-id="d8002-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8002-138">The following is an example of the response.</span></span> 
><span data-ttu-id="d8002-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8002-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
