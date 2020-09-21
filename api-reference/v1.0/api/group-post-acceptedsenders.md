---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b3f55e75d84a00622a0bc1d9fcda4e2aa2ddf535
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057537"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="c319d-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="c319d-103">Create acceptedSender</span></span>

<span data-ttu-id="c319d-104">Пространство имен: Microsoft. Graph Добавление нового пользователя или группы в список acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="c319d-104">Namespace: microsoft.graph Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="c319d-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="c319d-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="c319d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c319d-108">Permissions</span></span>
<span data-ttu-id="c319d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c319d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c319d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c319d-111">Permission type</span></span>      | <span data-ttu-id="c319d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c319d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c319d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c319d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c319d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c319d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c319d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c319d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c319d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c319d-116">Not supported.</span></span>    |
|<span data-ttu-id="c319d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c319d-117">Application</span></span> | <span data-ttu-id="c319d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c319d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c319d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c319d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c319d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c319d-120">Request headers</span></span>
| <span data-ttu-id="c319d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c319d-121">Header</span></span>       | <span data-ttu-id="c319d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c319d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c319d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c319d-123">Authorization</span></span>  | <span data-ttu-id="c319d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c319d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c319d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c319d-126">Request body</span></span>
<span data-ttu-id="c319d-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="c319d-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="c319d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c319d-128">Response</span></span>
<span data-ttu-id="c319d-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="c319d-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="c319d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c319d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c319d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c319d-131">Request</span></span>
<span data-ttu-id="c319d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c319d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c319d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c319d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c319d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c319d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c319d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c319d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c319d-136">C#</span><span class="sxs-lookup"><span data-stu-id="c319d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c319d-137">Java</span><span class="sxs-lookup"><span data-stu-id="c319d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acceptedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c319d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c319d-138">Response</span></span>
<span data-ttu-id="c319d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c319d-139">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

