---
title: 'group: renew'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 70f0ef9c40d5e23b80b5ba5c4f959369412137a1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277646"
---
# <a name="group-renew"></a><span data-ttu-id="ee562-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="ee562-104">group: renew</span></span>

<span data-ttu-id="ee562-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="ee562-105">Renews a group's expiration.</span></span> <span data-ttu-id="ee562-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="ee562-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee562-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee562-107">Permissions</span></span>

<span data-ttu-id="ee562-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee562-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="ee562-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee562-110">Permission type</span></span>      | <span data-ttu-id="ee562-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee562-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee562-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee562-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee562-113">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee562-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee562-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee562-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee562-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ee562-115">Not supported</span></span> |
|<span data-ttu-id="ee562-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee562-116">Application</span></span> | <span data-ttu-id="ee562-117">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee562-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee562-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee562-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="ee562-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee562-119">Request headers</span></span>
| <span data-ttu-id="ee562-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ee562-120">Name</span></span>       | <span data-ttu-id="ee562-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ee562-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee562-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee562-122">Authorization</span></span>  | <span data-ttu-id="ee562-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ee562-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="ee562-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee562-124">Request body</span></span>

<span data-ttu-id="ee562-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee562-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee562-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee562-126">Response</span></span>

<span data-ttu-id="ee562-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ee562-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee562-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ee562-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee562-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee562-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="ee562-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee562-131">Response</span></span>
<span data-ttu-id="ee562-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee562-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ee562-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ee562-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ee562-135">C#</span><span class="sxs-lookup"><span data-stu-id="ee562-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_renew-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee562-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee562-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_renew-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ee562-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ee562-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_renew-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
