---
title: Удаление события
description: Удаление объекта event.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5ea2b2e4803bfea38634dc7bfb367322987e5a54
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680992"
---
# <a name="delete-event"></a><span data-ttu-id="1df21-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="1df21-103">Delete event</span></span>

<span data-ttu-id="1df21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1df21-105">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1df21-105">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1df21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1df21-106">Permissions</span></span>
<span data-ttu-id="1df21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1df21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1df21-109">Permission type</span></span>      | <span data-ttu-id="1df21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1df21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1df21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1df21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1df21-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1df21-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1df21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1df21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1df21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df21-114">Not supported.</span></span>    |
|<span data-ttu-id="1df21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1df21-115">Application</span></span> | <span data-ttu-id="1df21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df21-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1df21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1df21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1df21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1df21-118">Request headers</span></span>
| <span data-ttu-id="1df21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1df21-119">Name</span></span>       | <span data-ttu-id="1df21-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1df21-120">Type</span></span> | <span data-ttu-id="1df21-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1df21-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1df21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1df21-122">Authorization</span></span>  | <span data-ttu-id="1df21-123">string</span><span class="sxs-lookup"><span data-stu-id="1df21-123">string</span></span>  | <span data-ttu-id="1df21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1df21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1df21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1df21-126">Request body</span></span>
<span data-ttu-id="1df21-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1df21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1df21-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df21-128">Response</span></span>
<span data-ttu-id="1df21-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1df21-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1df21-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1df21-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1df21-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df21-132">Request</span></span>
<span data-ttu-id="1df21-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1df21-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1df21-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df21-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="1df21-135">C#</span><span class="sxs-lookup"><span data-stu-id="1df21-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df21-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df21-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df21-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df21-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df21-138">Java</span><span class="sxs-lookup"><span data-stu-id="1df21-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1df21-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df21-139">Response</span></span>
<span data-ttu-id="1df21-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1df21-140">The following is an example of the response.</span></span> 
><span data-ttu-id="1df21-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1df21-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

