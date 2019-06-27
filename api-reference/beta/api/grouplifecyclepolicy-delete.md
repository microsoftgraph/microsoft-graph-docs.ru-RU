---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6e206a0d7fbee52c2262b2e8e85ee9d538692379
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262792"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="08aed-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="08aed-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08aed-104">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08aed-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08aed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08aed-105">Permissions</span></span>

<span data-ttu-id="08aed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08aed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08aed-108">Permission type</span></span>      | <span data-ttu-id="08aed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08aed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08aed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08aed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08aed-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08aed-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="08aed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08aed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08aed-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="08aed-113">Not supported</span></span> |
|<span data-ttu-id="08aed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08aed-114">Application</span></span> | <span data-ttu-id="08aed-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08aed-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08aed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08aed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="08aed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08aed-117">Request headers</span></span>

| <span data-ttu-id="08aed-118">Имя</span><span class="sxs-lookup"><span data-stu-id="08aed-118">Name</span></span> | <span data-ttu-id="08aed-119">Описание</span><span class="sxs-lookup"><span data-stu-id="08aed-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="08aed-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08aed-120">Authorization</span></span> | <span data-ttu-id="08aed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08aed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08aed-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08aed-123">Content-Type</span></span>  | <span data-ttu-id="08aed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08aed-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08aed-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08aed-125">Request body</span></span>
<span data-ttu-id="08aed-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08aed-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="08aed-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="08aed-127">Response</span></span>

<span data-ttu-id="08aed-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08aed-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08aed-130">Пример</span><span class="sxs-lookup"><span data-stu-id="08aed-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08aed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="08aed-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="08aed-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="08aed-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="08aed-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="08aed-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="08aed-134">C#</span><span class="sxs-lookup"><span data-stu-id="08aed-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08aed-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="08aed-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="08aed-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="08aed-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
