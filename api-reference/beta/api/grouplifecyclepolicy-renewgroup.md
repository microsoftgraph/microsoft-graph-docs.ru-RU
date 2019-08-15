---
title: 'groupLifecyclePolicy: Реневграуп'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d1cb4b602b3272ff27f635b84cf4a19b12739b9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419974"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="93b1f-104">groupLifecyclePolicy: Реневграуп</span><span class="sxs-lookup"><span data-stu-id="93b1f-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93b1f-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="93b1f-105">Renews a group's expiration.</span></span> <span data-ttu-id="93b1f-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="93b1f-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="93b1f-107">**Примечание:** В версии 1.0 [Используйте ресурс Group, чтобы выполнить обновление запросов](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="93b1f-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="93b1f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93b1f-108">Permissions</span></span>

<span data-ttu-id="93b1f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93b1f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="93b1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93b1f-111">Permission type</span></span>      | <span data-ttu-id="93b1f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93b1f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93b1f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93b1f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="93b1f-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93b1f-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="93b1f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93b1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93b1f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="93b1f-116">Not supported</span></span> |
|<span data-ttu-id="93b1f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93b1f-117">Application</span></span> | <span data-ttu-id="93b1f-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93b1f-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93b1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93b1f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="93b1f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93b1f-120">Request headers</span></span>

| <span data-ttu-id="93b1f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="93b1f-121">Name</span></span> | <span data-ttu-id="93b1f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="93b1f-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="93b1f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93b1f-123">Authorization</span></span> | <span data-ttu-id="93b1f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93b1f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93b1f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93b1f-126">Content-Type</span></span>  | <span data-ttu-id="93b1f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="93b1f-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="93b1f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93b1f-128">Request body</span></span>
<span data-ttu-id="93b1f-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="93b1f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93b1f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="93b1f-130">Parameter</span></span> | <span data-ttu-id="93b1f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93b1f-131">Type</span></span> | <span data-ttu-id="93b1f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93b1f-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="93b1f-133">groupId</span><span class="sxs-lookup"><span data-stu-id="93b1f-133">groupId</span></span>|<span data-ttu-id="93b1f-134">GUID</span><span class="sxs-lookup"><span data-stu-id="93b1f-134">Guid</span></span>| <span data-ttu-id="93b1f-135">Идентификатор группы, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="93b1f-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="93b1f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b1f-136">Response</span></span>

<span data-ttu-id="93b1f-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="93b1f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93b1f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="93b1f-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93b1f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="93b1f-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93b1f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="93b1f-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="93b1f-142">C#</span><span class="sxs-lookup"><span data-stu-id="93b1f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93b1f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93b1f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93b1f-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="93b1f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93b1f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b1f-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
