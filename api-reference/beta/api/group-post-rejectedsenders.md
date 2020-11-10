---
title: Создание объекта rejectedSender
description: Добавление пользователя или группы в список объектов rejectedSender.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dc5cbb68b67977ac0dc4c135587ef7b79fe5a8bc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964957"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="cf61b-103">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="cf61b-103">Create rejectedSender</span></span>

<span data-ttu-id="cf61b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf61b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf61b-105">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="cf61b-105">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="cf61b-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="cf61b-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf61b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf61b-109">Permissions</span></span>
<span data-ttu-id="cf61b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf61b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf61b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf61b-112">Permission type</span></span>      | <span data-ttu-id="cf61b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf61b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf61b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf61b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf61b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf61b-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf61b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf61b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf61b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf61b-117">Not supported.</span></span>    |
|<span data-ttu-id="cf61b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf61b-118">Application</span></span> | <span data-ttu-id="cf61b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf61b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf61b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf61b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cf61b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf61b-121">Request headers</span></span>
| <span data-ttu-id="cf61b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf61b-122">Header</span></span>       | <span data-ttu-id="cf61b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cf61b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf61b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf61b-124">Authorization</span></span>  | <span data-ttu-id="cf61b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf61b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf61b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf61b-127">Request body</span></span>
<span data-ttu-id="cf61b-128">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="cf61b-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="cf61b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf61b-129">Response</span></span>
<span data-ttu-id="cf61b-130">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="cf61b-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf61b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf61b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cf61b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf61b-132">Request</span></span>
<span data-ttu-id="cf61b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf61b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf61b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf61b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cf61b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf61b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf61b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf61b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf61b-137">C#</span><span class="sxs-lookup"><span data-stu-id="cf61b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf61b-138">Java</span><span class="sxs-lookup"><span data-stu-id="cf61b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf61b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf61b-139">Response</span></span>
<span data-ttu-id="cf61b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf61b-140">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


