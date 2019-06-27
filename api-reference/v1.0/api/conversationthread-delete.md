---
title: Удаление объекта conversationThread
description: Удаление объекта conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d08797d7b7068be794e1b6c6f4e915225017a69e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274713"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="44678-103">Удаление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="44678-103">Delete conversationThread</span></span>

<span data-ttu-id="44678-104">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="44678-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="44678-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44678-105">Permissions</span></span>
<span data-ttu-id="44678-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44678-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44678-108">Permission type</span></span>      | <span data-ttu-id="44678-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44678-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44678-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44678-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44678-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44678-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44678-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44678-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44678-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44678-113">Not supported.</span></span>    |
|<span data-ttu-id="44678-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44678-114">Application</span></span> | <span data-ttu-id="44678-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44678-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44678-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44678-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="44678-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44678-117">Request headers</span></span>
| <span data-ttu-id="44678-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44678-118">Header</span></span>       | <span data-ttu-id="44678-119">Значение</span><span class="sxs-lookup"><span data-stu-id="44678-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44678-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44678-120">Authorization</span></span>  | <span data-ttu-id="44678-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44678-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44678-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44678-123">Request body</span></span>
<span data-ttu-id="44678-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44678-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44678-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="44678-125">Response</span></span>

<span data-ttu-id="44678-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="44678-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44678-128">Пример</span><span class="sxs-lookup"><span data-stu-id="44678-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44678-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="44678-129">Request</span></span>
<span data-ttu-id="44678-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44678-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="44678-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="44678-131">Response</span></span>
<span data-ttu-id="44678-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44678-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="44678-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="44678-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="44678-134">C#</span><span class="sxs-lookup"><span data-stu-id="44678-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44678-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="44678-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="44678-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="44678-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
