---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ef3e1dd0e6280200d789c11659cd7d2ecd0f80ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263316"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="d1278-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="d1278-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1278-104">Удаление пользователя или группы из списка отклоненных отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="d1278-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1278-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1278-105">Permissions</span></span>
<span data-ttu-id="d1278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1278-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1278-108">Permission type</span></span>                        | <span data-ttu-id="d1278-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1278-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="d1278-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1278-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1278-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1278-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="d1278-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1278-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1278-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1278-113">Not supported.</span></span> |
| <span data-ttu-id="d1278-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1278-114">Application</span></span>                            | <span data-ttu-id="d1278-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1278-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1278-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1278-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="d1278-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1278-117">Request headers</span></span>

| <span data-ttu-id="d1278-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1278-118">Header</span></span>         | <span data-ttu-id="d1278-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d1278-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="d1278-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1278-120">Authorization</span></span>  | <span data-ttu-id="d1278-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1278-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="d1278-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1278-123">Request body</span></span>
<span data-ttu-id="d1278-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1278-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1278-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1278-125">Response</span></span>
<span data-ttu-id="d1278-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1278-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1278-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1278-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="d1278-129">Пример 1: Удаление пользователя из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="d1278-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="d1278-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1278-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a><span data-ttu-id="d1278-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1278-131">Response</span></span>
<span data-ttu-id="d1278-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1278-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1278-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d1278-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1278-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1278-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1278-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1278-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d1278-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d1278-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="d1278-137">Пример 2: Удаление группы из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="d1278-137">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="d1278-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1278-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="d1278-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1278-139">Response</span></span>
<span data-ttu-id="d1278-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1278-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1278-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d1278-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1278-142">C#</span><span class="sxs-lookup"><span data-stu-id="d1278-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1278-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1278-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d1278-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d1278-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
