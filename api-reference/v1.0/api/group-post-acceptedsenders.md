---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f98a98afe3fd0bb6c4e9aa72ee9b17de6882d8ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613765"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="ce16c-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="ce16c-103">Create acceptedSender</span></span>
<span data-ttu-id="ce16c-104">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="ce16c-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="ce16c-p101">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="ce16c-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce16c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce16c-108">Permissions</span></span>
<span data-ttu-id="ce16c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce16c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce16c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce16c-111">Permission type</span></span>      | <span data-ttu-id="ce16c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce16c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce16c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce16c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ce16c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce16c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce16c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce16c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce16c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce16c-116">Not supported.</span></span>    |
|<span data-ttu-id="ce16c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce16c-117">Application</span></span> | <span data-ttu-id="ce16c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce16c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce16c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce16c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ce16c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce16c-120">Request headers</span></span>
| <span data-ttu-id="ce16c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce16c-121">Header</span></span>       | <span data-ttu-id="ce16c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce16c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce16c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce16c-123">Authorization</span></span>  | <span data-ttu-id="ce16c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce16c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce16c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce16c-126">Request body</span></span>
<span data-ttu-id="ce16c-127">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="ce16c-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="ce16c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce16c-128">Response</span></span>
<span data-ttu-id="ce16c-129">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="ce16c-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce16c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ce16c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce16c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce16c-131">Request</span></span>
<span data-ttu-id="ce16c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce16c-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ce16c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce16c-133">Response</span></span>
<span data-ttu-id="ce16c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce16c-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce16c-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ce16c-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce16c-136">Язык</span><span class="sxs-lookup"><span data-stu-id="ce16c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_acceptedsender-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
