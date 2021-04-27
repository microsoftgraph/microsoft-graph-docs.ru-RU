---
title: Удаление события
description: Удаление объекта event.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ee3f41a979a15a2663c506734ac27011bc06d490
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042018"
---
# <a name="delete-event"></a><span data-ttu-id="5d184-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="5d184-103">Delete event</span></span>

<span data-ttu-id="5d184-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d184-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d184-105">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="5d184-105">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d184-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d184-106">Permissions</span></span>
<span data-ttu-id="5d184-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d184-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d184-109">Permission type</span></span>      | <span data-ttu-id="5d184-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d184-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d184-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d184-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d184-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d184-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d184-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d184-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d184-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d184-114">Not supported.</span></span>    |
|<span data-ttu-id="5d184-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d184-115">Application</span></span> | <span data-ttu-id="5d184-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d184-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d184-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d184-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d184-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d184-118">Request headers</span></span>
| <span data-ttu-id="5d184-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d184-119">Name</span></span>       | <span data-ttu-id="5d184-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5d184-120">Type</span></span> | <span data-ttu-id="5d184-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5d184-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d184-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d184-122">Authorization</span></span>  | <span data-ttu-id="5d184-123">string</span><span class="sxs-lookup"><span data-stu-id="5d184-123">string</span></span>  | <span data-ttu-id="5d184-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d184-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d184-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d184-126">Request body</span></span>
<span data-ttu-id="5d184-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d184-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d184-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d184-128">Response</span></span>
<span data-ttu-id="5d184-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5d184-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d184-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5d184-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5d184-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d184-132">Request</span></span>
<span data-ttu-id="5d184-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d184-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d184-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d184-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="5d184-135">C#</span><span class="sxs-lookup"><span data-stu-id="5d184-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d184-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d184-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d184-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d184-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d184-138">Java</span><span class="sxs-lookup"><span data-stu-id="5d184-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5d184-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d184-139">Response</span></span>
<span data-ttu-id="5d184-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d184-140">The following is an example of the response.</span></span> 
><span data-ttu-id="5d184-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d184-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


