---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ef2722aaf20dc2271b82525aa680410b98a45297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396724"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="941d0-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="941d0-103">Create acceptedSender</span></span>

<span data-ttu-id="941d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941d0-105">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="941d0-105">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="941d0-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="941d0-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="941d0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="941d0-109">Permissions</span></span>
<span data-ttu-id="941d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941d0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941d0-112">Permission type</span></span>      | <span data-ttu-id="941d0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="941d0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941d0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941d0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="941d0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941d0-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="941d0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941d0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941d0-117">Not supported.</span></span>    |
|<span data-ttu-id="941d0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941d0-118">Application</span></span> | <span data-ttu-id="941d0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941d0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="941d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941d0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="941d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941d0-121">Request headers</span></span>
| <span data-ttu-id="941d0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="941d0-122">Header</span></span>       | <span data-ttu-id="941d0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="941d0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="941d0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941d0-124">Authorization</span></span>  | <span data-ttu-id="941d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941d0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="941d0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="941d0-127">Request body</span></span>
<span data-ttu-id="941d0-128">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="941d0-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="941d0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="941d0-129">Response</span></span>
<span data-ttu-id="941d0-130">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="941d0-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="941d0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="941d0-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="941d0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="941d0-132">Request</span></span>
<span data-ttu-id="941d0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="941d0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="941d0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="941d0-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="941d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="941d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="941d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="941d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="941d0-137">C#</span><span class="sxs-lookup"><span data-stu-id="941d0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="941d0-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="941d0-138">Response</span></span>
<span data-ttu-id="941d0-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="941d0-139">The following is an example of the response.</span></span>
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
