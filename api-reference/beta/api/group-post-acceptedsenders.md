---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 827e6d12f8a237718993e49050cb7df2176b0637
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420667"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="43f65-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="43f65-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f65-104">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="43f65-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="43f65-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="43f65-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="43f65-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43f65-108">Permissions</span></span>
<span data-ttu-id="43f65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43f65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43f65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43f65-111">Permission type</span></span>      | <span data-ttu-id="43f65-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43f65-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43f65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43f65-113">Delegated (work or school account)</span></span> | <span data-ttu-id="43f65-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f65-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="43f65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43f65-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43f65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43f65-116">Not supported.</span></span>    |
|<span data-ttu-id="43f65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43f65-117">Application</span></span> | <span data-ttu-id="43f65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43f65-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43f65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43f65-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="43f65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43f65-120">Request headers</span></span>
| <span data-ttu-id="43f65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43f65-121">Header</span></span>       | <span data-ttu-id="43f65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43f65-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="43f65-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43f65-123">Authorization</span></span>  | <span data-ttu-id="43f65-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43f65-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43f65-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43f65-126">Request body</span></span>
<span data-ttu-id="43f65-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="43f65-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="43f65-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="43f65-128">Response</span></span>
<span data-ttu-id="43f65-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="43f65-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f65-130">Пример</span><span class="sxs-lookup"><span data-stu-id="43f65-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="43f65-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43f65-131">Request</span></span>
<span data-ttu-id="43f65-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43f65-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="43f65-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="43f65-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43f65-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43f65-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43f65-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="43f65-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="43f65-136">C#</span><span class="sxs-lookup"><span data-stu-id="43f65-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="43f65-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="43f65-137">Response</span></span>
<span data-ttu-id="43f65-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43f65-138">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
