---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b46893b52b7d82d7b9ab8fbda1029a9acfa3dc31
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262974"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="75b43-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="75b43-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b43-104">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="75b43-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="75b43-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="75b43-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="75b43-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75b43-108">Permissions</span></span>
<span data-ttu-id="75b43-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75b43-111">Permission type</span></span>      | <span data-ttu-id="75b43-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75b43-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75b43-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75b43-113">Delegated (work or school account)</span></span> | <span data-ttu-id="75b43-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b43-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75b43-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75b43-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75b43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b43-116">Not supported.</span></span>    |
|<span data-ttu-id="75b43-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75b43-117">Application</span></span> | <span data-ttu-id="75b43-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b43-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75b43-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75b43-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="75b43-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75b43-120">Request headers</span></span>
| <span data-ttu-id="75b43-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75b43-121">Header</span></span>       | <span data-ttu-id="75b43-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75b43-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75b43-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75b43-123">Authorization</span></span>  | <span data-ttu-id="75b43-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75b43-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75b43-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75b43-126">Request body</span></span>
<span data-ttu-id="75b43-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="75b43-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="75b43-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="75b43-128">Response</span></span>
<span data-ttu-id="75b43-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="75b43-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b43-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75b43-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="75b43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="75b43-131">Request</span></span>
<span data-ttu-id="75b43-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75b43-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="75b43-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="75b43-133">Response</span></span>
<span data-ttu-id="75b43-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75b43-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="75b43-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="75b43-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75b43-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="75b43-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_acceptedsender-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="75b43-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75b43-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_acceptedsender-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-post-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
