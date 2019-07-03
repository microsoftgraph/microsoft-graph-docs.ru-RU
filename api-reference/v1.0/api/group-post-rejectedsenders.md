---
title: Создание объекта rejectedSender
description: Добавление пользователя или группы в список объектов rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9174ed775c0b03f7e329a8e4c0e8ee9c2fe60ece
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456381"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="3425c-103">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="3425c-103">Create rejectedSender</span></span>
<span data-ttu-id="3425c-104">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="3425c-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="3425c-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="3425c-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="3425c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3425c-108">Permissions</span></span>
<span data-ttu-id="3425c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3425c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3425c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3425c-111">Permission type</span></span>      | <span data-ttu-id="3425c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3425c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3425c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3425c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3425c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3425c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3425c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3425c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3425c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3425c-116">Not supported.</span></span>    |
|<span data-ttu-id="3425c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3425c-117">Application</span></span> | <span data-ttu-id="3425c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3425c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3425c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3425c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3425c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3425c-120">Request headers</span></span>
| <span data-ttu-id="3425c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3425c-121">Header</span></span>       | <span data-ttu-id="3425c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3425c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3425c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3425c-123">Authorization</span></span>  | <span data-ttu-id="3425c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3425c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3425c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3425c-126">Request body</span></span>
<span data-ttu-id="3425c-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="3425c-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="3425c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3425c-128">Response</span></span>
<span data-ttu-id="3425c-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="3425c-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="3425c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3425c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3425c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3425c-131">Request</span></span>
<span data-ttu-id="3425c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3425c-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3425c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3425c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3425c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3425c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3425c-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3425c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3425c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3425c-136">Response</span></span>
<span data-ttu-id="3425c-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3425c-137">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
