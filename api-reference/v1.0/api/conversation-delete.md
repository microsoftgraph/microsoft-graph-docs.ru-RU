---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: af498b79b42e4f56d8ed9c9ca5897cc0f2e1a03b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273838"
---
# <a name="delete-conversation"></a><span data-ttu-id="40752-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="40752-103">Delete conversation</span></span>

<span data-ttu-id="40752-104">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="40752-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="40752-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40752-105">Permissions</span></span>
<span data-ttu-id="40752-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40752-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40752-108">Permission type</span></span>      | <span data-ttu-id="40752-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40752-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40752-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40752-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40752-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40752-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40752-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40752-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40752-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40752-113">Not supported.</span></span>    |
|<span data-ttu-id="40752-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40752-114">Application</span></span> | <span data-ttu-id="40752-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40752-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40752-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40752-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40752-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40752-117">Request headers</span></span>
| <span data-ttu-id="40752-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40752-118">Header</span></span>       | <span data-ttu-id="40752-119">Значение</span><span class="sxs-lookup"><span data-stu-id="40752-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40752-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40752-120">Authorization</span></span>  | <span data-ttu-id="40752-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40752-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40752-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40752-123">Request body</span></span>
<span data-ttu-id="40752-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40752-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40752-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="40752-125">Response</span></span>

<span data-ttu-id="40752-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="40752-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40752-128">Пример</span><span class="sxs-lookup"><span data-stu-id="40752-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40752-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="40752-129">Request</span></span>
<span data-ttu-id="40752-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40752-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="40752-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="40752-131">Response</span></span>
<span data-ttu-id="40752-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40752-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="40752-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="40752-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="40752-134">C#</span><span class="sxs-lookup"><span data-stu-id="40752-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40752-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="40752-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="40752-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="40752-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_conversation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
