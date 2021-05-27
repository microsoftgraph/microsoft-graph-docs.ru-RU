---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 31a4dd44eb0f16b78dfe3b2cebe068ba825e6835
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681419"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="1e9c2-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="1e9c2-103">Create acceptedSender</span></span>

<span data-ttu-id="1e9c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e9c2-105">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-105">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="1e9c2-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e9c2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e9c2-109">Permissions</span></span>
<span data-ttu-id="1e9c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e9c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e9c2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e9c2-112">Permission type</span></span>      | <span data-ttu-id="1e9c2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e9c2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e9c2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e9c2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1e9c2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9c2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e9c2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e9c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e9c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-117">Not supported.</span></span>    |
|<span data-ttu-id="1e9c2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e9c2-118">Application</span></span> | <span data-ttu-id="1e9c2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e9c2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e9c2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1e9c2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e9c2-121">Request headers</span></span>
| <span data-ttu-id="1e9c2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e9c2-122">Header</span></span>       | <span data-ttu-id="1e9c2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1e9c2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e9c2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e9c2-124">Authorization</span></span>  | <span data-ttu-id="1e9c2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e9c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e9c2-127">Request body</span></span>
<span data-ttu-id="1e9c2-128">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="1e9c2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e9c2-129">Response</span></span>
<span data-ttu-id="1e9c2-130">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e9c2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e9c2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1e9c2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e9c2-132">Request</span></span>
<span data-ttu-id="1e9c2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e9c2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e9c2-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1e9c2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e9c2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e9c2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e9c2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1e9c2-137">C#</span><span class="sxs-lookup"><span data-stu-id="1e9c2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e9c2-138">Java</span><span class="sxs-lookup"><span data-stu-id="1e9c2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acceptedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1e9c2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e9c2-139">Response</span></span>
<span data-ttu-id="1e9c2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1e9c2-140">The following is an example of the response.</span></span>
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


