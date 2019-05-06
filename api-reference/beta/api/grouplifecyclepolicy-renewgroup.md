---
title: 'groupLifecyclePolicy: Реневграуп'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5815d7d12677419fc04cbfd383c8456c0b26e180
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592327"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="0c4c3-104">groupLifecyclePolicy: Реневграуп</span><span class="sxs-lookup"><span data-stu-id="0c4c3-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c4c3-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-105">Renews a group's expiration.</span></span> <span data-ttu-id="0c4c3-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="0c4c3-107">**Примечание:** В версии 1.0 [Используйте ресурс Group, чтобы выполнить обновление запросов](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="0c4c3-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4c3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4c3-108">Permissions</span></span>

<span data-ttu-id="0c4c3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="0c4c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4c3-111">Permission type</span></span>      | <span data-ttu-id="0c4c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4c3-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4c3-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c4c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4c3-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c4c3-116">Not supported</span></span> |
|<span data-ttu-id="0c4c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4c3-117">Application</span></span> | <span data-ttu-id="0c4c3-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4c3-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4c3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="0c4c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4c3-120">Request headers</span></span>

| <span data-ttu-id="0c4c3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4c3-121">Name</span></span> | <span data-ttu-id="0c4c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4c3-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="0c4c3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c4c3-123">Authorization</span></span> | <span data-ttu-id="0c4c3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c4c3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c4c3-126">Content-Type</span></span>  | <span data-ttu-id="0c4c3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4c3-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c4c3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c4c3-128">Request body</span></span>
<span data-ttu-id="0c4c3-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c4c3-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c4c3-130">Parameter</span></span> | <span data-ttu-id="0c4c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4c3-131">Type</span></span> | <span data-ttu-id="0c4c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4c3-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0c4c3-133">groupId</span><span class="sxs-lookup"><span data-stu-id="0c4c3-133">groupId</span></span>|<span data-ttu-id="0c4c3-134">GUID</span><span class="sxs-lookup"><span data-stu-id="0c4c3-134">Guid</span></span>| <span data-ttu-id="0c4c3-135">Идентификатор группы, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="0c4c3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4c3-136">Response</span></span>

<span data-ttu-id="0c4c3-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c4c3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4c3-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4c3-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0c4c3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4c3-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="0c4c3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4c3-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c4c3-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0c4c3-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c4c3-143">Языках</span><span class="sxs-lookup"><span data-stu-id="0c4c3-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c4c3-144">Язык</span><span class="sxs-lookup"><span data-stu-id="0c4c3-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
