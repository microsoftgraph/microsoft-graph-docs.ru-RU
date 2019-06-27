---
title: Создание объекта rejectedSender
description: Добавление пользователя или группы в список объектов rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dd92d188b580a56ab45374eb9d59bec851a2e3a8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277667"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="6ecbd-103">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="6ecbd-103">Create rejectedSender</span></span>
<span data-ttu-id="6ecbd-104">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="6ecbd-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ecbd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecbd-108">Permissions</span></span>
<span data-ttu-id="6ecbd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecbd-111">Permission type</span></span>      | <span data-ttu-id="6ecbd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ecbd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ecbd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ecbd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ecbd-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ecbd-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ecbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ecbd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ecbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-116">Not supported.</span></span>    |
|<span data-ttu-id="6ecbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ecbd-117">Application</span></span> | <span data-ttu-id="6ecbd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ecbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ecbd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6ecbd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ecbd-120">Request headers</span></span>
| <span data-ttu-id="6ecbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ecbd-121">Header</span></span>       | <span data-ttu-id="6ecbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ecbd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ecbd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ecbd-123">Authorization</span></span>  | <span data-ttu-id="6ecbd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ecbd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ecbd-126">Request body</span></span>
<span data-ttu-id="6ecbd-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="6ecbd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecbd-128">Response</span></span>
<span data-ttu-id="6ecbd-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ecbd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6ecbd-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6ecbd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecbd-131">Request</span></span>
<span data-ttu-id="6ecbd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-132">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="6ecbd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecbd-133">Response</span></span>
<span data-ttu-id="6ecbd-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecbd-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ecbd-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6ecbd-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ecbd-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ecbd-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6ecbd-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6ecbd-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
