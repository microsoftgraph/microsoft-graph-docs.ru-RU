---
title: 'group: renew'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8f77eb80bed4188299aedf1efd0b6800975f38ac
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613657"
---
# <a name="group-renew"></a><span data-ttu-id="10097-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="10097-104">group: renew</span></span>

<span data-ttu-id="10097-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="10097-105">Renews a group's expiration.</span></span> <span data-ttu-id="10097-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="10097-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="10097-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10097-107">Permissions</span></span>

<span data-ttu-id="10097-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10097-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="10097-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10097-110">Permission type</span></span>      | <span data-ttu-id="10097-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10097-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10097-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10097-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10097-113">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10097-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="10097-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10097-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10097-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10097-115">Not supported</span></span> |
|<span data-ttu-id="10097-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10097-116">Application</span></span> | <span data-ttu-id="10097-117">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10097-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10097-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10097-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="10097-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10097-119">Request headers</span></span>
| <span data-ttu-id="10097-120">Имя</span><span class="sxs-lookup"><span data-stu-id="10097-120">Name</span></span>       | <span data-ttu-id="10097-121">Описание</span><span class="sxs-lookup"><span data-stu-id="10097-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="10097-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10097-122">Authorization</span></span>  | <span data-ttu-id="10097-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10097-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="10097-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10097-124">Request body</span></span>

<span data-ttu-id="10097-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10097-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10097-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="10097-126">Response</span></span>

<span data-ttu-id="10097-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="10097-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10097-129">Пример</span><span class="sxs-lookup"><span data-stu-id="10097-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10097-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="10097-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="10097-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="10097-131">Response</span></span>
<span data-ttu-id="10097-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10097-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="10097-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="10097-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10097-135">Языках</span><span class="sxs-lookup"><span data-stu-id="10097-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_renew-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10097-136">Язык</span><span class="sxs-lookup"><span data-stu-id="10097-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_renew-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
