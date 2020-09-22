---
title: 'groupLifecyclePolicy: Реневграуп'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1421a2ffa62935c8b16ba8d8e3126e3d3cede770
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001829"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="2364d-104">groupLifecyclePolicy: Реневграуп</span><span class="sxs-lookup"><span data-stu-id="2364d-104">groupLifecyclePolicy: renewGroup</span></span>

<span data-ttu-id="2364d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2364d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2364d-106">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="2364d-106">Renews a group's expiration.</span></span> <span data-ttu-id="2364d-107">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="2364d-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="2364d-108">**Примечание:** В версии 1.0 [Используйте ресурс Group, чтобы выполнить обновление запросов](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="2364d-108">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="2364d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2364d-109">Permissions</span></span>

<span data-ttu-id="2364d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2364d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="2364d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2364d-112">Permission type</span></span>      | <span data-ttu-id="2364d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2364d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2364d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2364d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2364d-115">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2364d-115">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2364d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2364d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2364d-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2364d-117">Not supported</span></span> |
|<span data-ttu-id="2364d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2364d-118">Application</span></span> | <span data-ttu-id="2364d-119">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2364d-119">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2364d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2364d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="2364d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2364d-121">Request headers</span></span>

| <span data-ttu-id="2364d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2364d-122">Name</span></span> | <span data-ttu-id="2364d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2364d-123">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2364d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2364d-124">Authorization</span></span> | <span data-ttu-id="2364d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2364d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2364d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2364d-127">Content-Type</span></span>  | <span data-ttu-id="2364d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2364d-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2364d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2364d-129">Request body</span></span>
<span data-ttu-id="2364d-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2364d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2364d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="2364d-131">Parameter</span></span> | <span data-ttu-id="2364d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2364d-132">Type</span></span> | <span data-ttu-id="2364d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2364d-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2364d-134">groupId</span><span class="sxs-lookup"><span data-stu-id="2364d-134">groupId</span></span>|<span data-ttu-id="2364d-135">GUID</span><span class="sxs-lookup"><span data-stu-id="2364d-135">Guid</span></span>| <span data-ttu-id="2364d-136">Идентификатор группы, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="2364d-136">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="2364d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2364d-137">Response</span></span>

<span data-ttu-id="2364d-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2364d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2364d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2364d-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2364d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2364d-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2364d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2364d-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2364d-143">C#</span><span class="sxs-lookup"><span data-stu-id="2364d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2364d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2364d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2364d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2364d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2364d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2364d-146">Response</span></span>

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


