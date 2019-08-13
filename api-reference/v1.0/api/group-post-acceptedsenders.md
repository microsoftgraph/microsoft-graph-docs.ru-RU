---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: eafe458bc9e290a982395efe21cc2d87a29a4411
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337176"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="46c54-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="46c54-103">Create acceptedSender</span></span>
<span data-ttu-id="46c54-104">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="46c54-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="46c54-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="46c54-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="46c54-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46c54-108">Permissions</span></span>
<span data-ttu-id="46c54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46c54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46c54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46c54-111">Permission type</span></span>      | <span data-ttu-id="46c54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46c54-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46c54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46c54-113">Delegated (work or school account)</span></span> | <span data-ttu-id="46c54-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46c54-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46c54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46c54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46c54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46c54-116">Not supported.</span></span>    |
|<span data-ttu-id="46c54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46c54-117">Application</span></span> | <span data-ttu-id="46c54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46c54-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46c54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46c54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="46c54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46c54-120">Request headers</span></span>
| <span data-ttu-id="46c54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46c54-121">Header</span></span>       | <span data-ttu-id="46c54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46c54-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="46c54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46c54-123">Authorization</span></span>  | <span data-ttu-id="46c54-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46c54-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46c54-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46c54-126">Request body</span></span>
<span data-ttu-id="46c54-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="46c54-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="46c54-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="46c54-128">Response</span></span>
<span data-ttu-id="46c54-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="46c54-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c54-130">Пример</span><span class="sxs-lookup"><span data-stu-id="46c54-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="46c54-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="46c54-131">Request</span></span>
<span data-ttu-id="46c54-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46c54-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46c54-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="46c54-133">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46c54-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46c54-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46c54-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46c54-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="46c54-136">C#</span><span class="sxs-lookup"><span data-stu-id="46c54-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46c54-137">Java</span><span class="sxs-lookup"><span data-stu-id="46c54-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acceptedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46c54-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="46c54-138">Response</span></span>
<span data-ttu-id="46c54-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="46c54-139">The following is an example of the response.</span></span>
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
